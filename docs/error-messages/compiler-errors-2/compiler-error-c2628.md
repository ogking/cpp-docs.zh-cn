---
title: 编译器错误 C2628
ms.date: 11/04/2016
f1_keywords:
- C2628
helpviewer_keywords:
- C2628
ms.assetid: 19a25e77-d5be-4107-88d5-0745b6281f98
ms.openlocfilehash: 90df41ba8ae85e57e40848f8b50f4c1df7c7b541
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50664940"
---
# <a name="compiler-error-c2628"></a>编译器错误 C2628

type1 和 type2 是非法的 (是否忘记了;？)

可能缺少分号。

下面的示例生成 C2628:

```
// C2628.cpp
class CMyClass {}
int main(){}   // C2628 error
```

可能的解决方法：

```
// C2628b.cpp
class CMyClass {};
int main(){}
```