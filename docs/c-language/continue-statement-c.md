---
title: continue 语句 (C)
ms.date: 11/04/2016
f1_keywords:
- continue
helpviewer_keywords:
- loop structures, continue keyword
- continue keyword [C]
ms.assetid: 969f293a-45fe-48a7-b4c6-287ba27a631d
ms.openlocfilehash: db3ed1d1575a52b8d54466f763f348821c458f31
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50587157"
---
# <a name="continue-statement-c"></a>continue 语句 (C)

`continue` 语句将控制传递给它在其中出现的最近的封闭 `do`、`for` 或 `while` 语句的下一个迭代，并绕过 `do`、`for` 或 `while` 语句主体中的任何剩余语句。

## <a name="syntax"></a>语法

*jump-statement*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**continue ;**

确定 `do`、`for` 或 `while` 语句的下一次迭代，如下所示：

- 在 `do` 或 `while` 语句中，下一个迭代首先会重新计算 `do` 或 `while` 语句的表达式。

- `continue` 语句中的 `for` 语句会导致计算 `for` 语句的循环表达式。 然后，编译器会重新计算条件表达式并根据结果终止或迭代语句主体。 有关 `for` 语句及其非终止符的详细信息，请参阅 [for 语句](../c-language/for-statement-c.md)。

以下是 `continue` 语句的示例：

```
while ( i-- > 0 )
{
    x = f( i );
    if ( x == 1 )
        continue;
    y += x * x;
}
```

在此示例中，当 `i` 大于 0 时，将执行语句主体。 首先将 `f(i)` 赋给 `x`；然后，如果 `x` 等于 1，则执行 `continue` 语句。 主体中的语句的其余部分将被忽略，并且执行将通过计算循环的测试来基于循环恢复。

## <a name="see-also"></a>请参阅

[continue 语句](../cpp/continue-statement-cpp.md)