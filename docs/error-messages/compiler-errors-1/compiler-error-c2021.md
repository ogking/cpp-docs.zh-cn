---
title: 编译器错误 C2021
ms.date: 11/04/2016
f1_keywords:
- C2021
helpviewer_keywords:
- C2021
ms.assetid: 064f32e2-3794-48d5-9767-991003dcb36a
ms.openlocfilehash: 6492dfffbb5a2f80ea543d4248c0f77759c0a521
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50513995"
---
# <a name="compiler-error-c2021"></a>编译器错误 C2021

应输入指数值而非“character”

用作浮点常数的指数的字符不是有效数字。 请务必使用在范围内的指数。

## <a name="example"></a>示例

下面的示例生成 C2021:

```
// C2021.cpp
float test1=1.175494351E;   // C2021
```

## <a name="example"></a>示例

可能的解决方法：

```
// C2021b.cpp
// compile with: /c
float test2=1.175494351E8;
```