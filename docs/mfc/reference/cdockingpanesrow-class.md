---
title: CDockingPanesRow 类
ms.date: 10/18/2018
f1_keywords:
- CDockingPanesRow
- AFXDOCKINGPANESROW/CDockingPanesRow
- AFXDOCKINGPANESROW/CDockingPanesRow::AddPane
- AFXDOCKINGPANESROW/CDockingPanesRow::AddPaneFromRow
- AFXDOCKINGPANESROW/CDockingPanesRow::ArrangePanes
- AFXDOCKINGPANESROW/CDockingPanesRow::CalcFixedLayout
- AFXDOCKINGPANESROW/CDockingPanesRow::Create
- AFXDOCKINGPANESROW/CDockingPanesRow::ExpandStretchedPanes
- AFXDOCKINGPANESROW/CDockingPanesRow::ExpandStretchedPanesRect
- AFXDOCKINGPANESROW/CDockingPanesRow::FixupVirtualRects
- AFXDOCKINGPANESROW/CDockingPanesRow::GetAvailableLength
- AFXDOCKINGPANESROW/CDockingPanesRow::GetAvailableSpace
- AFXDOCKINGPANESROW/CDockingPanesRow::GetClientRect
- AFXDOCKINGPANESROW/CDockingPanesRow::GetDockSite
- AFXDOCKINGPANESROW/CDockingPanesRow::GetExtraSpace
- AFXDOCKINGPANESROW/CDockingPanesRow::GetGroupFromPane
- AFXDOCKINGPANESROW/CDockingPanesRow::GetID
- AFXDOCKINGPANESROW/CDockingPanesRow::GetMaxPaneSize
- AFXDOCKINGPANESROW/CDockingPanesRow::GetPaneCount
- AFXDOCKINGPANESROW/CDockingPanesRow::GetPaneList
- AFXDOCKINGPANESROW/CDockingPanesRow::GetRowAlignment
- AFXDOCKINGPANESROW/CDockingPanesRow::GetRowHeight
- AFXDOCKINGPANESROW/CDockingPanesRow::GetRowOffset
- AFXDOCKINGPANESROW/CDockingPanesRow::GetVisibleCount
- AFXDOCKINGPANESROW/CDockingPanesRow::GetWindowRect
- AFXDOCKINGPANESROW/CDockingPanesRow::HasPane
- AFXDOCKINGPANESROW/CDockingPanesRow::IsEmpty
- AFXDOCKINGPANESROW/CDockingPanesRow::IsExclusiveRow
- AFXDOCKINGPANESROW/CDockingPanesRow::IsHorizontal
- AFXDOCKINGPANESROW/CDockingPanesRow::IsVisible
- AFXDOCKINGPANESROW/CDockingPanesRow::Move
- AFXDOCKINGPANESROW/CDockingPanesRow::MovePane
- AFXDOCKINGPANESROW/CDockingPanesRow::OnResizePane
- AFXDOCKINGPANESROW/CDockingPanesRow::RedrawAll
- AFXDOCKINGPANESROW/CDockingPanesRow::RemovePane
- AFXDOCKINGPANESROW/CDockingPanesRow::ReplacePane
- AFXDOCKINGPANESROW/CDockingPanesRow::RepositionPanes
- AFXDOCKINGPANESROW/CDockingPanesRow::Resize
- AFXDOCKINGPANESROW/CDockingPanesRow::ResizeByPaneDivider
- AFXDOCKINGPANESROW/CDockingPanesRow::ScreenToClient
- AFXDOCKINGPANESROW/CDockingPanesRow::SetExtra
- AFXDOCKINGPANESROW/CDockingPanesRow::ShowDockSiteRow
- AFXDOCKINGPANESROW/CDockingPanesRow::ShowPane
- AFXDOCKINGPANESROW/CDockingPanesRow::UpdateVisibleState
helpviewer_keywords:
- CDockingPanesRow [MFC], AddPane
- CDockingPanesRow [MFC], AddPaneFromRow
- CDockingPanesRow [MFC], ArrangePanes
- CDockingPanesRow [MFC], CalcFixedLayout
- CDockingPanesRow [MFC], Create
- CDockingPanesRow [MFC], ExpandStretchedPanes
- CDockingPanesRow [MFC], ExpandStretchedPanesRect
- CDockingPanesRow [MFC], FixupVirtualRects
- CDockingPanesRow [MFC], GetAvailableLength
- CDockingPanesRow [MFC], GetAvailableSpace
- CDockingPanesRow [MFC], GetClientRect
- CDockingPanesRow [MFC], GetDockSite
- CDockingPanesRow [MFC], GetExtraSpace
- CDockingPanesRow [MFC], GetGroupFromPane
- CDockingPanesRow [MFC], GetID
- CDockingPanesRow [MFC], GetMaxPaneSize
- CDockingPanesRow [MFC], GetPaneCount
- CDockingPanesRow [MFC], GetPaneList
- CDockingPanesRow [MFC], GetRowAlignment
- CDockingPanesRow [MFC], GetRowHeight
- CDockingPanesRow [MFC], GetRowOffset
- CDockingPanesRow [MFC], GetVisibleCount
- CDockingPanesRow [MFC], GetWindowRect
- CDockingPanesRow [MFC], HasPane
- CDockingPanesRow [MFC], IsEmpty
- CDockingPanesRow [MFC], IsExclusiveRow
- CDockingPanesRow [MFC], IsHorizontal
- CDockingPanesRow [MFC], IsVisible
- CDockingPanesRow [MFC], Move
- CDockingPanesRow [MFC], MovePane
- CDockingPanesRow [MFC], OnResizePane
- CDockingPanesRow [MFC], RedrawAll
- CDockingPanesRow [MFC], RemovePane
- CDockingPanesRow [MFC], ReplacePane
- CDockingPanesRow [MFC], RepositionPanes
- CDockingPanesRow [MFC], Resize
- CDockingPanesRow [MFC], ResizeByPaneDivider
- CDockingPanesRow [MFC], ScreenToClient
- CDockingPanesRow [MFC], SetExtra
- CDockingPanesRow [MFC], ShowDockSiteRow
- CDockingPanesRow [MFC], ShowPane
- CDockingPanesRow [MFC], UpdateVisibleState
ms.assetid: e7a17832-0ebb-4bce-b799-cec9b60f76fe
ms.openlocfilehash: a2d9c7894327a66c24fae3890856dbb95a6d10e4
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50450123"
---
# <a name="cdockingpanesrow-class"></a>CDockingPanesRow 类

管理位于停靠站点中同一水平或垂直行（列）的窗格的列表。

有关更多详细信息，请参阅中的源代码**VC\\atlmfc\\src\\mfc**的 Visual Studio 安装文件夹。

## <a name="syntax"></a>语法

```
class CDockingPanesRow : public CObject
```

## <a name="members"></a>成员

### <a name="public-constructors"></a>公共构造函数

|名称|描述|
|----------|-----------------|
|`CDockingPanesRow::CDockingPanesRow`|默认构造函数。|

### <a name="public-methods"></a>公共方法

|名称|描述|
|----------|-----------------|
|[CDockingPanesRow::AddPane](#addpane)||
|[CDockingPanesRow::AddPaneFromRow](#addpanefromrow)||
|[CDockingPanesRow::ArrangePanes](#arrangepanes)|根据指定边距和间距参数将窗格排成行。|
|[CDockingPanesRow::CalcFixedLayout](#calcfixedlayout)||
|[CDockingPanesRow::Create](#create)||
|[CDockingPanesRow::ExpandStretchedPanes](#expandstretchedpanes)||
|[CDockingPanesRow::ExpandStretchedPanesRect](#expandstretchedpanesrect)||
|[CDockingPanesRow::FixupVirtualRects](#fixupvirtualrects)||
|[CDockingPanesRow::GetAvailableLength](#getavailablelength)||
|[CDockingPanesRow::GetAvailableSpace](#getavailablespace)||
|[CDockingPanesRow::GetClientRect](#getclientrect)||
|[CDockingPanesRow::GetDockSite](#getdocksite)||
|[CDockingPanesRow::GetExtraSpace](#getextraspace)||
|[CDockingPanesRow::GetGroupFromPane](#getgroupfrompane)||
|[CDockingPanesRow::GetID](#getid)||
|[CDockingPanesRow::GetMaxPaneSize](#getmaxpanesize)||
|[CDockingPanesRow::GetPaneCount](#getpanecount)||
|[CDockingPanesRow::GetPaneList](#getpanelist)||
|[CDockingPanesRow::GetRowAlignment](#getrowalignment)||
|[CDockingPanesRow::GetRowHeight](#getrowheight)||
|[CDockingPanesRow::GetRowOffset](#getrowoffset)||
|[CDockingPanesRow::GetVisibleCount](#getvisiblecount)||
|[CDockingPanesRow::GetWindowRect](#getwindowrect)||
|[CDockingPanesRow::HasPane](#haspane)||
|[CDockingPanesRow::IsEmpty](#isempty)||
|[CDockingPanesRow::IsExclusiveRow](#isexclusiverow)||
|[CDockingPanesRow::IsHorizontal](#ishorizontal)||
|[CDockingPanesRow::IsVisible](#isvisible)||
|[CDockingPanesRow::Move](#move)||
|[CDockingPanesRow::MovePane](#movepane)||
|[CDockingPanesRow::OnResizePane](#onresizepane)||
|[CDockingPanesRow::RedrawAll](#redrawall)||
|[CDockingPanesRow::RemovePane](#removepane)||
|[CDockingPanesRow::ReplacePane](#replacepane)||
|[CDockingPanesRow::RepositionPanes](#repositionpanes)||
|[CDockingPanesRow::Resize](#resize)||
|[CDockingPanesRow::ResizeByPaneDivider](#resizebypanedivider)||
|[CDockingPanesRow::ScreenToClient](#screentoclient)||
|[CDockingPanesRow::SetExtra](#setextra)||
|[CDockingPanesRow::ShowDockSiteRow](#showdocksiterow)||
|[CDockingPanesRow::ShowPane](#showpane)||
|[CDockingPanesRow::UpdateVisibleState](#updatevisiblestate)||

## <a name="remarks"></a>备注

`CDockingPanesRow` 对象由停靠站点对象在内部创建。

## <a name="example"></a>示例

下面的示例演示如何从 `CMFCAutoHideBar` 对象获取 `CDockingPanesRow` 对象。

[!code-cpp[NVC_MFC_RibbonApp#26](../../mfc/reference/codesnippet/cpp/cdockingpanesrow-class_1.cpp)]

## <a name="inheritance-hierarchy"></a>继承层次结构

[CObject](../../mfc/reference/cobject-class.md)

[CDockingPanesRow](../../mfc/reference/cdockingpanesrow-class.md)

## <a name="requirements"></a>要求

**标头：** afxDockingPanesRow.h

##  <a name="addpane"></a>  CDockingPanesRow::AddPane

```
virtual void AddPane(
    CPane* pControlBar,
    AFX_DOCK_METHOD dockMethod,
    LPCRECT lpRect = NULL,
    BOOL bAddLast = FALSE);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

[in]*dockMethod*<br/>

[in]*lpRect*<br/>

[in]*bAddLast*<br/>

### <a name="remarks"></a>备注

##  <a name="addpanefromrow"></a>  CDockingPanesRow::AddPaneFromRow

```
virtual void AddPaneFromRow(
    CPane* pControlBar,
    AFX_DOCK_METHOD dockMethod);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

[in]*dockMethod*<br/>

### <a name="remarks"></a>备注

##  <a name="arrangepanes"></a>  CDockingPanesRow::ArrangePanes

排列停靠窗格根据指定边距和间距参数。

```
virtual void ArrangePanes(
    int nMargin,
    int nSpacing);
```

### <a name="parameters"></a>参数

*nMargin*<br/>
[in]指定的偏移量，以像素为单位从左上角的行的第一个窗格。

*nSpacing*<br/>
[in]指定以像素为单位的窗格之间的间距。

### <a name="remarks"></a>备注

调用此方法来排列中的行，它们将停靠的窗格。 调用此方法后，必须调用`CDockingPanesRow::FixupVirtualRects(FALSE, NULL)`。

##  <a name="calcfixedlayout"></a>  CDockingPanesRow::CalcFixedLayout

```
virtual CSize CalcFixedLayout(
    BOOL bStretch,
    BOOL bHorz);
```

### <a name="parameters"></a>参数

[in]*bStretch*<br/>

[in]*bHorz*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="cdockingpanesrow"></a>  CDockingPanesRow::CDockingPanesRow

```
CDockingPanesRow(
    CDockSite* pParentDockBar,
    int nOffset,
    int nHeight);
```

### <a name="parameters"></a>参数

[in]*pParentDockBar*<br/>

[in]*nOffset*<br/>

[in]*nHeight*<br/>

### <a name="remarks"></a>备注

##  <a name="create"></a>  CDockingPanesRow::Create

```
virtual BOOL Create();
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="expandstretchedpanes"></a>  CDockingPanesRow::ExpandStretchedPanes

```
void ExpandStretchedPanes();
```

### <a name="remarks"></a>备注

##  <a name="expandstretchedpanesrect"></a>  CDockingPanesRow::ExpandStretchedPanesRect

```
void ExpandStretchedPanesRect();
```

### <a name="remarks"></a>备注

##  <a name="fixupvirtualrects"></a>  CDockingPanesRow::FixupVirtualRects

```
void FixupVirtualRects(
    bool bMoveBackToVirtualRect,
    CPane* pBarToExclude = NULL);
```

### <a name="parameters"></a>参数

[in]*bMoveBackToVirtualRect*<br/>

[in]*pBarToExclude*<br/>

### <a name="remarks"></a>备注

##  <a name="getavailablelength"></a>  CDockingPanesRow::GetAvailableLength

```
virtual int GetAvailableLength(BOOL bUseVirtualRect = FALSE) const;
```

### <a name="parameters"></a>参数

[in]*bUseVirtualRect*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getavailablespace"></a>  CDockingPanesRow::GetAvailableSpace

```
virtual void GetAvailableSpace(CRect& rect);
```

### <a name="parameters"></a>参数

[in]*rect*<br/>

### <a name="remarks"></a>备注

##  <a name="getclientrect"></a>  CDockingPanesRow::GetClientRect

```
void GetClientRect(CRect& rect) const;
```

### <a name="parameters"></a>参数

[in]*rect*<br/>

### <a name="remarks"></a>备注

##  <a name="getdocksite"></a>  CDockingPanesRow::GetDockSite

```
CDockSite* GetDockSite() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getextraspace"></a>  CDockingPanesRow::GetExtraSpace

```
int GetExtraSpace() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getgroupfrompane"></a>  CDockingPanesRow::GetGroupFromPane

```
void GetGroupFromPane(
    CPane* pBar,
    CObList& lst);
```

### <a name="parameters"></a>参数

[in]*pBar*<br/>

[in]*lst*<br/>

### <a name="remarks"></a>备注

##  <a name="getid"></a>  CDockingPanesRow::GetID

```
int GetID() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getmaxpanesize"></a>  CDockingPanesRow::GetMaxPaneSize

```
int GetMaxPaneSize(BOOL bSkipHiddenBars = TRUE) const;
```

### <a name="parameters"></a>参数

[in]*bSkipHiddenBars*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getpanecount"></a>  CDockingPanesRow::GetPaneCount

```
int GetPaneCount() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getpanelist"></a>  CDockingPanesRow::GetPaneList

```
const CObList& GetPaneList() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getrowalignment"></a>  CDockingPanesRow::GetRowAlignment

```
DWORD GetRowAlignment() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getrowheight"></a>  CDockingPanesRow::GetRowHeight

```
int GetRowHeight() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getrowoffset"></a>  CDockingPanesRow::GetRowOffset

```
int GetRowOffset() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getvisiblecount"></a>  CDockingPanesRow::GetVisibleCount

```
virtual int GetVisibleCount();
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="getwindowrect"></a>  CDockingPanesRow::GetWindowRect

```
void GetWindowRect(CRect& rect) const;
```

### <a name="parameters"></a>参数

[in]*rect*<br/>

### <a name="remarks"></a>备注

##  <a name="haspane"></a>  CDockingPanesRow::HasPane

```
BOOL HasPane(CBasePane* pControlBar);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="isempty"></a>  CDockingPanesRow::IsEmpty

```
virtual BOOL IsEmpty() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="isexclusiverow"></a>  CDockingPanesRow::IsExclusiveRow

```
virtual BOOL IsExclusiveRow() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="ishorizontal"></a>  CDockingPanesRow::IsHorizontal

```
bool IsHorizontal() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="isvisible"></a>  CDockingPanesRow::IsVisible

```
virtual BOOL IsVisible() const;
```

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="move"></a>  CDockingPanesRow::Move

```
virtual void Move(int nOffset);
```

### <a name="parameters"></a>参数

[in]*nOffset*<br/>

### <a name="remarks"></a>备注

##  <a name="movepane"></a>  CDockingPanesRow::MovePane

```
void MovePane(
    CPane* pControlBar,
    CPoint ptOffset,
    BOOL bSwapControlBars,
    HDWP& hdwp);

void MovePane(
    CPane* pControlBar,
    CRect rectTarget,
    HDWP& hdwp);

void MovePane(
    CPane* pControlBar,
    int nOffset,
    bool bForward,
    HDWP& hdwp);

void MovePane(
    CPane* pControlBar,
    int nAbsolutOffset,
    HDWP& hdwp);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

[in]*ptOffset*<br/>

[in]*bSwapControlBars*<br/>

[in]*hdwp*<br/>

[in]*rectTarget*<br/>

[in]*nOffset*<br/>

[in]*bForward*<br/>

[in]*nAbsolutOffset*<br/>

### <a name="remarks"></a>备注

##  <a name="onresizepane"></a>  CDockingPanesRow::OnResizePane

```
virtual void OnResizePane(CBasePane* pControlBar);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

### <a name="remarks"></a>备注

##  <a name="redrawall"></a>  CDockingPanesRow::RedrawAll

```
void RedrawAll();
```

### <a name="remarks"></a>备注

##  <a name="removepane"></a>  CDockingPanesRow::RemovePane

```
virtual void RemovePane(CPane* pControlBar);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

### <a name="remarks"></a>备注

##  <a name="replacepane"></a>  CDockingPanesRow::ReplacePane

```
virtual BOOL ReplacePane(
    CPane* pBarOld,
    CPane* pBarNew);
```

### <a name="parameters"></a>参数

[in]*pBarOld*<br/>

[in]*pBarNew*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="repositionpanes"></a>  CDockingPanesRow::RepositionPanes

```
virtual void RepositionPanes(
    CRect& rectNewParentBarArea,
    UINT nSide = (UINT)-1,
    BOOL bExpand = FALSE,
    int nOffset = 0);
```

### <a name="parameters"></a>参数

[in]*rectNewParentBarArea*<br/>

[in]*深入剖析*<br/>

[in]*bExpand*<br/>

[in]*nOffset*<br/>

### <a name="remarks"></a>备注

##  <a name="resize"></a>  CDockingPanesRow::Resize

```
virtual int Resize(int nOffset);
```

### <a name="parameters"></a>参数

[in]*nOffset*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="resizebypanedivider"></a>  CDockingPanesRow::ResizeByPaneDivider

```
virtual int ResizeByPaneDivider(int /*ignored*/);
```

### <a name="parameters"></a>参数

[in]*忽略*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="screentoclient"></a>  CDockingPanesRow::ScreenToClient

```
void ScreenToClient(CRect& rect) const;
```

### <a name="parameters"></a>参数

[in]*rect*<br/>

### <a name="remarks"></a>备注

##  <a name="setextra"></a>  CDockingPanesRow::SetExtra

```
void SetExtra(
    int nExtraSpace,
    AFX_ROW_ALIGNMENT rowExtraAlign);
```

### <a name="parameters"></a>参数

[in]*nExtraSpace*<br/>

[in]*rowExtraAlign*<br/>

### <a name="remarks"></a>备注

##  <a name="showdocksiterow"></a>  CDockingPanesRow::ShowDockSiteRow

```
virtual void ShowDockSiteRow(
    BOOL bShow,
    BOOL bDelay);
```

### <a name="parameters"></a>参数

[in]*bShow*<br/>

[in]*bDelay*<br/>

### <a name="remarks"></a>备注

##  <a name="showpane"></a>  CDockingPanesRow::ShowPane

```
virtual BOOL ShowPane(
    CPane* pControlBar,
    BOOL bShow,
    BOOL bDelay = FALSE);
```

### <a name="parameters"></a>参数

[in]*pControlBar*<br/>

[in]*bShow*<br/>

[in]*bDelay*<br/>

### <a name="return-value"></a>返回值

### <a name="remarks"></a>备注

##  <a name="updatevisiblestate"></a>  CDockingPanesRow::UpdateVisibleState

```
virtual void UpdateVisibleState(BOOL bDelay);
```

### <a name="parameters"></a>参数

[in]*bDelay*<br/>

### <a name="remarks"></a>备注

## <a name="see-also"></a>请参阅

[层次结构图](../../mfc/hierarchy-chart.md)<br/>
[类](../../mfc/reference/mfc-classes.md)<br/>
[CObject 类](../../mfc/reference/cobject-class.md)<br/>
[CDockSite 类](../../mfc/reference/cdocksite-class.md)<br/>
[CPane 类](../../mfc/reference/cpane-class.md)
