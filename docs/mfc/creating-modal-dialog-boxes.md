---
title: 创建模式对话框
ms.date: 11/04/2016
helpviewer_keywords:
- modal dialog boxes [MFC], creating
- MFC dialog boxes [MFC], creating
- MFC dialog boxes [MFC], modal
ms.assetid: 26c7a68c-79f6-4862-a5a8-6024984644d2
ms.openlocfilehash: eb9aab7e8579fbbbfdf5d0f2dca9b6e6abea0066
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50657326"
---
# <a name="creating-modal-dialog-boxes"></a>创建模式对话框

若要创建模式对话框，请调用中声明的两个公共构造函数之一[CDialog](../mfc/reference/cdialog-class.md)。 接下来，调用对话框对象的[DoModal](../mfc/reference/cdialog-class.md#domodal)成员函数以显示该对话框并管理与之交互，直到用户选择确定或取消。 正是由 `DoModal` 进行的上述管理工作使得对话框成为模式对话框。 对于模式对话框，`DoModal` 将加载对话框资源。

## <a name="see-also"></a>请参阅

[对话框的生命周期](../mfc/life-cycle-of-a-dialog-box.md)

