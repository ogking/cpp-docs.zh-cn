---
title: '@（指定编译器响应文件）'
ms.date: 11/04/2016
f1_keywords:
- '@'
helpviewer_keywords:
- response files, C/C++ compiler
- '@ compiler option'
- cl.exe compiler, specifying response files
ms.assetid: 400fffee-909d-4f60-bf76-45833e822685
ms.openlocfilehash: 90dcadbb47cdc7eb4fa1ff039f5074a3141eac83
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50491307"
---
# <a name="-specify-a-compiler-response-file"></a>@（指定编译器响应文件）

指定编译器响应文件。

## <a name="syntax"></a>语法

> **\@**<em>response_file</em>

## <a name="arguments"></a>自变量

*response_file*<br/>
包含编译器的命令的文本文件。

## <a name="remarks"></a>备注

响应文件可以包含将在命令行指定任何命令。 如果命令行自变量超过 127 个字符，这可能很有用。

不能指定**\@** 选项响应文件中。 也就是说，响应文件不能嵌入另一个响应文件。

从命令行中，您可以指定任意多个响应文件选项 (例如， `@respfile.1 @respfile.2`) 所需。

### <a name="to-set-this-compiler-option-in-the-visual-studio-development-environment"></a>在 Visual Studio 开发环境中设置此编译器选项

- 响应文件不能从开发环境中指定，也必须在命令行指定。

### <a name="to-set-this-compiler-option-programmatically"></a>以编程方式设置此编译器选项

- 不能以编程方式更改此编译器选项。

## <a name="see-also"></a>请参阅

[编译器选项](../../build/reference/compiler-options.md)<br/>
[设置编译器选项](../../build/reference/setting-compiler-options.md)
