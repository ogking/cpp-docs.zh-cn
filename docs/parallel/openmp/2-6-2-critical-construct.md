---
title: 2.6.2 critical 构造
ms.date: 11/04/2016
ms.assetid: c46ecd00-b4a2-4a5e-ba92-288c329e773a
ms.openlocfilehash: dcc0e6144be5daee2a225cda621db818e5a38e2c
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50539069"
---
# <a name="262-critical-construct"></a>2.6.2 critical 构造

**关键**指令标识相关联的结构化块执行一个线程限制一次的构造。 语法**关键**指令是按如下所示：

```
#pragma omp critical [(name)]  new-linestructured-block
```

一个可选*名称*可能用于标识的关键区域。 标识符用于标识的关键区域具有外部链接，这不同于使用的标签、 标记、 成员和普通标识符的命名空间的命名空间中。

关键区域的开始处的一个线程等待，直到没有其他线程执行 （任意位置中程序） 具有相同名称的一个关键区域。 所有未命名**关键**指令将映射到相同的未指定名称。