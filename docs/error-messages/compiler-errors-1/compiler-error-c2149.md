---
title: 编译器错误 C2149
ms.date: 11/04/2016
f1_keywords:
- C2149
helpviewer_keywords:
- C2149
ms.assetid: 7a106dab-d79f-41b9-85be-f36e86e4d2ab
ms.openlocfilehash: 62eca9730b28f83cea39d5c6606d4bb94ce885dd
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50445898"
---
# <a name="compiler-error-c2149"></a>编译器错误 C2149

“identifier”：已命名位域不能具有零宽度

位域只有在未命名时才可以有零宽度。

下面的示例生成 C2149：

```
// C2149.cpp
// compile with: /c
struct C {
   int i : 0;   // C2149
   int j : 2;   // OK
};
```