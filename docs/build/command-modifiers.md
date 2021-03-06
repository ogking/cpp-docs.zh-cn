---
title: 命令修饰符
ms.date: 11/04/2016
helpviewer_keywords:
- NMAKE program, command modifiers
- command modifiers
ms.assetid: b661c432-210f-4f05-bc56-744a46e0fc0b
ms.openlocfilehash: a9a79364880cf95adca6066b48f0d786391c8ba0
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50431807"
---
# <a name="command-modifiers"></a>命令修饰符

可以指定前面的命令，可以选择用空格或制表符分隔的一个或多个命令修饰符。 与命令一样，必须缩进修饰符。

|修饰符|目标|
|--------------|-------------|
|\@*命令*|禁止显示该命令。 不取消显示由命令。 默认情况下，NMAKE 回显所有执行的命令。 使用 /S 取消显示整个生成文件;使用 **。无提示**取消生成文件的一部分显示。|
|**-**\[*数字*]*命令*|关闭的错误检查*命令*。 默认情况下，当命令返回非零退出代码时，NMAKE 暂停。 如果-*数量*是使用，NMAKE 停止如果退出代码超过*数*。 空格或制表符不能出现之间短划线和*数。* 之间必须有至少一个空格或制表符`number`并*命令*。 使用 /I 关闭检查整个生成文件; 时出错使用 **。忽略**关闭检查生成文件的一部分时出错。|
|**\!** *command*|执行*命令*为每个依赖文件如果*命令*使用<strong>$ \* \*</strong> （在依赖项中的所有依赖文件） 或 **$?** （所有依赖文件中更高版本的时间戳比目标对象的依赖项）。|

## <a name="see-also"></a>请参阅

[生成文件中的命令](../build/commands-in-a-makefile.md)
