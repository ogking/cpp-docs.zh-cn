---
title: 编译器警告 （等级 1） C4114
ms.date: 11/04/2016
f1_keywords:
- C4114
helpviewer_keywords:
- C4114
ms.assetid: 3983e1c6-e8bb-46dc-8894-e1827db48797
ms.openlocfilehash: 41e951e7c4a8b23ddbec14c5421f66702e70c937
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50450968"
---
# <a name="compiler-warning-level-1-c4114"></a>编译器警告 （等级 1） C4114

多次使用同一类型限定符

类型声明或定义使用类型限定符 (**const**，**易失性**，**签名**，或者**无符号**) 不止一次。 这将导致具有 Microsoft 扩展 (/Ze) 的警告和 ANSI 兼容性 (/Za) 错误。

下面的示例生成 C4114:

```
// C4114.cpp
// compile with: /W1 /c
volatile volatile int i;   // C4114
```

下面的示例生成 C4114:

```
// C4114_b.cpp
// compile with: /W1 /c
static const int const * ii;   // C4114
static const int * const iii;   // OK
```
