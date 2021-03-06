---
title: 对话框类
ms.date: 11/04/2016
f1_keywords:
- vc.classes.dialog
helpviewer_keywords:
- property sheet classes
- dialog box classes
- OLE common dialog classes
- common dialog classes [MFC]
- tab dialog boxes
ms.assetid: db75da23-4eff-4c6c-beae-79cf046fbce9
ms.openlocfilehash: 3533a548f009a65462ce0d821d782db0ada9aa4b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50489997"
---
# <a name="dialog-box-classes"></a>对话框类

类`CDialog`和及其派生的类封装对话框功能。 对话框是一种特殊的窗口中，由于`CDialog`派生自`CWnd`。 派生对话框类从`CDialog`或使用其中一个的标准对话框，如打开或保存文件、 打印、 选择的字体或颜色，通用对话框类启动搜索和替换操作，或执行各种 OLE 相关操作。

[CDialog](../mfc/reference/cdialog-class.md)<br/>
所有对话框，模式和无模式的基类。

[CDataExchange](../mfc/reference/cdataexchange-class.md)<br/>
提供对话框数据交换和验证的信息。

## <a name="common-dialogs"></a>通用对话框

这些对话框类封装 Windows 公共对话框。 它们提供易于使用的复杂的对话框实现。

[CCommonDialog](../mfc/reference/ccommondialog-class.md)<br/>
所有公共对话框的基类。

[CFileDialog](../mfc/reference/cfiledialog-class.md)<br/>
打开或保存文件中提供的标准对话框。

[CColorDialog](../mfc/reference/ccolordialog-class.md)<br/>
提供的标准对话框用于选择一种颜色。

[CFontDialog](../mfc/reference/cfontdialog-class.md)<br/>
提供用于选择字体的标准对话框。

[CFindReplaceDialog](../mfc/reference/cfindreplacedialog-class.md)<br/>
搜索和替换操作提供的标准对话框。

[CPrintDialog](../mfc/reference/cprintdialog-class.md)<br/>
提供用于打印文件的标准对话框。

[CPrintDialogEx](../mfc/reference/cprintdialogex-class.md)<br/>
提供 Windows 打印属性表。

[CPageSetupDialog](../mfc/reference/cpagesetupdialog-class.md)<br/>
封装由 Windows 公共页面设置对话框提供与其他支持，用于设置和修改打印边距的服务。

## <a name="ole-common-dialogs"></a>OLE 通用对话框

OLE 将几个通用对话框添加到 Windows。 这些类封装了 OLE 通用对话框。

[COleDialog](../mfc/reference/coledialog-class.md)<br/>
由框架使用，旨在包含所有 OLE 对话框的常见实现。 用户界面类别中的所有对话框类都派生自此基类。 `COleDialog` 无法直接使用。

[COleInsertDialog](../mfc/reference/coleinsertdialog-class.md)<br/>
显示“插入对象”对话框，即用于插入新的 OLE 链接项或嵌入项的标准用户界面。

[COlePasteSpecialDialog](../mfc/reference/colepastespecialdialog-class.md)<br/>
显示“选择性粘贴”对话框，即用于实现“编辑选择性粘贴”命令的标准用户界面。

[COleLinksDialog](../mfc/reference/colelinksdialog-class.md)<br/>
显示“编辑链接”对话框，即用于修改有关链接项的信息的标准用户界面。

[COleChangeIconDialog](../mfc/reference/colechangeicondialog-class.md)<br/>
显示“更改图标”对话框，即用于更改与 OLE 嵌入项或链接项关联的图标的标准用户界面。

[COleConvertDialog](../mfc/reference/coleconvertdialog-class.md)<br/>
显示“转换”对话框，即用于将 OLE 项从一种类型转换为另一种类型的标准用户界面。

[COlePropertiesDialog](../mfc/reference/colepropertiesdialog-class.md)<br/>
封装“Windows 公共 OLE 属性”对话框。 “公共 OLE 属性”对话框提供了一个简单方法，使您能够采用与 Windows 标准一致的方式来显示和修改 OLE 文档项的属性。

[COleUpdateDialog](../mfc/reference/coleupdatedialog-class.md)<br/>
显示“更新”对话框，即用于更新文档中的所有链接的标准用户界面。 对话框包含一个进度指示器，用来指示更新过程还有多久完成。

[COleChangeSourceDialog](../mfc/reference/colechangesourcedialog-class.md)<br/>
显示“更改源”对话框，即用于更改链接的目标或源的标准用户界面。

[COleBusyDialog](../mfc/reference/colebusydialog-class.md)<br/>
显示“服务器忙”和“服务器不响应”对话框，即用于处理对繁忙的应用程序的调用的标准用户界面。 通常会自动显示[COleMessageFilter](../mfc/reference/colemessagefilter-class.md)实现。

## <a name="property-sheet-classes"></a>属性表类

属性表类允许应用程序以使用属性表，也称为选项卡式对话框。 属性表是用于组织大量的单个对话框中控件的有效方式。

[CPropertyPage](../mfc/reference/cpropertypage-class.md)<br/>
提供了属性表内的各个页面。 从派生类`CPropertyPage`为每个页后，可以添加到属性表。

[CPropertySheet](../mfc/reference/cpropertysheet-class.md)<br/>
为多个属性页中提供的框架。 派生属性表类从`CPropertySheet`来快速实现属性表。

[COlePropertyPage](../mfc/reference/colepropertypage-class.md)<br/>
显示图形界面（与对话框类似）中的 OLE 控件的属性。

## <a name="html-based-dialog-classes"></a>基于 HTML 的对话框类

[CDHtmlDialog](../mfc/reference/cdhtmldialog-class.md)<br/>
用于创建实现用户界面与 HTML 而不是对话框资源的对话框。

[CMultiPageDHtmlDialog](../mfc/reference/cmultipagedhtmldialog-class.md)<br/>
按顺序显示多个 HTML 页，并处理来自每个页面的事件。

## <a name="related-classes"></a>相关的类

这些类不是对话框本身，但它们使用对话框模板，并且具有很多对话框的行为。

[CDialogBar](../mfc/reference/cdialogbar-class.md)<br/>
一个基于对话框模板的控件条。

[CFormView](../mfc/reference/cformview-class.md)<br/>
在对话框模板中定义其布局滚动视图。 从派生类`CFormView`以实现基于对话框模板的用户界面。

[CDaoRecordView](../mfc/reference/cdaorecordview-class.md)<br/>
提供了一种直接连接到数据访问对象 (DAO) 记录集对象的视图。 像所有窗体视图中，`CDaoRecordView`基于对话框模板。

[CRecordView](../mfc/reference/crecordview-class.md)<br/>
提供了一种直接连接到开放式数据库连接 (ODBC) 记录集对象的视图。 像所有窗体视图中，`CRecordView`基于对话框模板。

[CPrintInfo](../mfc/reference/cprintinfo-structure.md)<br/>
包含有关打印或打印预览作业的信息的结构。 使用的打印体系结构[CView](../mfc/reference/cview-class.md)。

## <a name="see-also"></a>请参阅

[类概述](../mfc/class-library-overview.md)

