---
title: 转换：诊断
ms.date: 11/04/2016
ms.assetid: 3730ca7c-0147-452d-bd4a-6a1e97e9793e
ms.openlocfilehash: 4863b97dc1db7ff295b5f786ca97da2551d0fa62
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50664992"
---
# <a name="translation-diagnostics"></a>转换：诊断

**ANSI 2.1.1.3** 如何标识诊断

Microsoft C 生成以下形式的错误消息：

> *filename* **(** *line-number* **) :** *diagnostic* **C**<em>number</em> *message*

其中，filename 是出现错误的源文件的名称；line-number 是编译器在其中检测到错误的行号；diagnostic 是“错误”或“警告”；number 是标识错误或警告的唯一的四位数（前面带有 C，如语法中所注明的）；message 是解释性消息。

## <a name="see-also"></a>请参阅

[实现定义的行为](../c-language/implementation-defined-behavior.md)