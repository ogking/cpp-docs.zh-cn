---
title: /doc（处理文档注释）(C/C++)
ms.date: 11/04/2016
f1_keywords:
- VC.Project.VCCLCompilerTool.GenerateXMLDocumentationFiles
- /doc
- VC.Project.VCCLCompilerTool.XMLDocumentationFileName
helpviewer_keywords:
- /doc compiler option [C++]
- comments, C++ code
- XML documentation, comments in source files
- -doc compiler option [C++]
ms.assetid: b54f7e2c-f28f-4f46-9ed6-0db09be2cc63
ms.openlocfilehash: 39b614b1ab21a654a35e30b0d3acffa15d244fb0
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50530034"
---
# <a name="doc-process-documentation-comments-cc"></a>/doc（处理文档注释）(C/C++)

在源代码文件，以创建用于每个源代码文件，其中包含文档注释的.xdc 文件可让编译器处理文档注释。

## <a name="syntax"></a>语法

> **/doc**[*名称*]

## <a name="arguments"></a>自变量

*name*<br/>
编译器会创建.xdc 文件的名称。 仅当在编译中传递一个.cpp 文件时才有效。

## <a name="remarks"></a>备注

.Xdc 文件处理到具有 xdcmake.exe 的.xml 文件。 有关详细信息，请参阅[XDCMake 参考](../../ide/xdcmake-reference.md)。

可以将文档注释添加到源代码文件。 有关详细信息，请参阅 [建议的文档注释标记](../../ide/recommended-tags-for-documentation-comments-visual-cpp.md)。

若要生成的.xml 文件中使用 IntelliSense，请与你想要支持，并将.xml 文件的程序集也是与程序集相同的目录中的.xml 文件的文件名。 当 Visual Studio 项目中引用该程序集时，会还会找到.xml 文件。 有关详细信息，请参阅[使用 IntelliSense](/visualstudio/ide/using-intellisense)并[提供 XML 代码注释](/visualstudio/ide/supplying-xml-code-comments)。

### <a name="to-set-this-compiler-option-in-the-visual-studio-development-environment"></a>在 Visual Studio 开发环境中设置此编译器选项

1. 打开项目的“属性页”  对话框。 有关详细信息，请参阅[使用项目属性](../../ide/working-with-project-properties.md)。

1. 选择**配置属性** > **C/c + +** > **输出文件**属性页。

1. 修改**生成 XML 文档文件**属性。

### <a name="to-set-this-linker-option-programmatically"></a>以编程方式设置此链接器选项

- 请参阅 <xref:Microsoft.VisualStudio.VCProjectEngine.VCCLCompilerTool.GenerateXMLDocumentationFiles%2A>。

## <a name="see-also"></a>请参阅

[编译器选项](../../build/reference/compiler-options.md)<br/>
[设置编译器选项](../../build/reference/setting-compiler-options.md)