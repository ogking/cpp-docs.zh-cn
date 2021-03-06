---
title: 编译器错误 C3068
ms.date: 11/04/2016
f1_keywords:
- C3068
helpviewer_keywords:
- C3068
ms.assetid: 613e3447-b4a8-4268-a661-297bed63ccdf
ms.openlocfilehash: 4790c9caafd28722f3631104cfe5cfc762cf6426
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50575469"
---
# <a name="compiler-error-c3068"></a>编译器错误 C3068

function: naked 函数不能包含会要求回退如果出现 c + + 异常的对象

编译器无法执行堆栈展开上[裸](../../cpp/naked-cpp.md)引发了异常，因为在函数和 c + + 异常处理中创建临时对象的函数 ([/EHsc](../../build/reference/eh-exception-handling-model.md)) 指定。

若要解决此错误，请执行在至少一个以下操作：

- 使用 /EHsc 不编译。

- 不要将标记为函数`naked`。

- 不要在函数中创建临时对象。

如果函数在堆栈上创建临时对象，如果该函数将引发异常，并启用 c + + 异常处理，编译器将清理堆栈如果引发异常。

时引发异常，编译器生成的代码，称为 prolog 和 epilog 和其中不存在的裸函数中，执行的函数。

## <a name="example"></a>示例

下面的示例生成 C3068:

```
// C3068.cpp
// compile with: /EHsc
// processor: x86
class A {
public:
   A(){}
   ~A(){}
};

void b(A){}

__declspec(naked) void c() {
   b(A());   // C3068
};
```