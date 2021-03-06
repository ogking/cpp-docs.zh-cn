---
title: 管理菜单、控件条和快捷键
ms.date: 11/04/2016
helpviewer_keywords:
- MDI [MFC], frame windows
- control bars [MFC], updating in frame windows
- menus [MFC], updating as context changes
- user interface objects [MFC], updating
- accelerator tables [MFC]
- sharing menus [MFC]
- updating user-interface objects [MFC]
- frame windows [MFC], updating
- status bars [MFC], updating
ms.assetid: 97ca1997-06df-4373-b023-4f7ecd81047b
ms.openlocfilehash: 905a015de6a675de80c49991750f72eccf06afaa
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50559622"
---
# <a name="managing-menus-control-bars-and-accelerators"></a>管理菜单、控件条和快捷键

框架窗口管理对用户界面对象（包括菜单、工具栏按钮、状态栏和快捷键）的更新。 它还管理对 MDI 应用程序中的菜单栏的共享。

## <a name="managing-menus"></a>管理菜单

框架窗口出现在中，更新用户界面项使用 ON_UPDATE_COMMAND_UI 机制中所述[如何更新用户界面对象](../mfc/how-to-update-user-interface-objects.md)。 空循环期间，工具栏上的按钮和其他控件栏会进行更新。 菜单栏上的下拉菜单中的菜单项正好在菜单下拉之前进行更新。

对于 MDI 应用程序，MDI 框架窗口管理菜单栏和标题。 MDI 框架窗口拥有一个默认菜单，该菜单可在没有活动 MDI 子窗口时用作菜单栏。 当存在活动子窗口时，MDI 框架窗口的菜单栏就会由活动的 MDI 子窗口取代。 如果 MDI 应用程序支持多个文档类型（如图表和工作表文档），则每个类型会将其自己的菜单放入菜单栏中并更改主框架窗口的标题。

[CMDIFrameWnd](../mfc/reference/cmdiframewnd-class.md)为 MDI 应用程序上显示的窗口菜单提供的标准命令的默认实现。 具体而言，实现新的窗口命令 (ID_WINDOW_NEW) 是为了创建新的框架窗口和当前文档的视图。 仅在需要高级自定义时重写这些实现。

同一文档类型的多个 MDI 子窗口共享菜单资源。 如果多个 MDI 子窗口是由同一个文档模板创建的，则它们可使用同一个菜单资源，并保存在 Windows 系统资源中。

## <a name="managing-the-status-bar"></a>管理状态栏

框架窗口还将状态栏置于其客户端区域内并管理状态栏的指示符。 框架窗口中清除和根据需要更新状态栏中的消息区域，并显示提示字符串，在用户选择菜单项或工具栏按钮，如中所述[如何在状态栏中显示命令信息](../mfc/how-to-display-command-information-in-the-status-bar.md)。

## <a name="managing-accelerators"></a>管理快捷键

每个框架窗口维护一个可选的快捷键表，此表可自动为您转换键盘快捷键。 利用该机制，可轻松定义调用菜单命令的快捷键。

## <a name="see-also"></a>请参阅

[使用框架窗口](../mfc/using-frame-windows.md)

