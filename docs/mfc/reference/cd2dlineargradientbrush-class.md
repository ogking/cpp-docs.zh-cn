---
title: CD2DLinearGradientBrush 类
ms.date: 11/04/2016
f1_keywords:
- CD2DLinearGradientBrush
- AFXRENDERTARGET/CD2DLinearGradientBrush
- AFXRENDERTARGET/CD2DLinearGradientBrush::CD2DLinearGradientBrush
- AFXRENDERTARGET/CD2DLinearGradientBrush::Attach
- AFXRENDERTARGET/CD2DLinearGradientBrush::Create
- AFXRENDERTARGET/CD2DLinearGradientBrush::Destroy
- AFXRENDERTARGET/CD2DLinearGradientBrush::Detach
- AFXRENDERTARGET/CD2DLinearGradientBrush::Get
- AFXRENDERTARGET/CD2DLinearGradientBrush::GetEndPoint
- AFXRENDERTARGET/CD2DLinearGradientBrush::GetStartPoint
- AFXRENDERTARGET/CD2DLinearGradientBrush::SetEndPoint
- AFXRENDERTARGET/CD2DLinearGradientBrush::SetStartPoint
- AFXRENDERTARGET/CD2DLinearGradientBrush::m_LinearGradientBrushProperties
- AFXRENDERTARGET/CD2DLinearGradientBrush::m_pLinearGradientBrush
helpviewer_keywords:
- CD2DLinearGradientBrush [MFC], CD2DLinearGradientBrush
- CD2DLinearGradientBrush [MFC], Attach
- CD2DLinearGradientBrush [MFC], Create
- CD2DLinearGradientBrush [MFC], Destroy
- CD2DLinearGradientBrush [MFC], Detach
- CD2DLinearGradientBrush [MFC], Get
- CD2DLinearGradientBrush [MFC], GetEndPoint
- CD2DLinearGradientBrush [MFC], GetStartPoint
- CD2DLinearGradientBrush [MFC], SetEndPoint
- CD2DLinearGradientBrush [MFC], SetStartPoint
- CD2DLinearGradientBrush [MFC], m_LinearGradientBrushProperties
- CD2DLinearGradientBrush [MFC], m_pLinearGradientBrush
ms.assetid: d4be9ff9-0ea8-45e6-9b8d-f3bc5673cbac
ms.openlocfilehash: 03c370be5bcfc61e1dd398604f27313d3de15f8b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50635814"
---
# <a name="cd2dlineargradientbrush-class"></a>CD2DLinearGradientBrush 类

ID2D1LinearGradientBrush 包装器。

## <a name="syntax"></a>语法

```
class CD2DLinearGradientBrush : public CD2DGradientBrush;
```

## <a name="members"></a>成员

### <a name="public-constructors"></a>公共构造函数

|名称|描述|
|----------|-----------------|
|[CD2DLinearGradientBrush::CD2DLinearGradientBrush](#cd2dlineargradientbrush)|构造一个 CD2DLinearGradientBrush 对象。|
|[CD2DLinearGradientBrush:: ~ CD2DLinearGradientBrush](#_dtorcd2dlineargradientbrush)|析构函数。 当 D2D 线性渐变画笔对象被销毁时调用。|

### <a name="public-methods"></a>公共方法

|名称|描述|
|----------|-----------------|
|[CD2DLinearGradientBrush::Attach](#attach)|附加现有的资源的对象的接口|
|[CD2DLinearGradientBrush::Create](#create)|创建 CD2DLinearGradientBrush。 (重写[CD2DResource::Create](../../mfc/reference/cd2dresource-class.md#create)。)|
|[CD2DLinearGradientBrush::Destroy](#destroy)|销毁 CD2DLinearGradientBrush 对象。 (重写[CD2DGradientBrush::Destroy](../../mfc/reference/cd2dgradientbrush-class.md#destroy)。)|
|[CD2DLinearGradientBrush::Detach](#detach)|分离对象中的资源接口|
|[CD2DLinearGradientBrush::Get](#get)|返回 ID2D1LinearGradientBrush 接口|
|[CD2DLinearGradientBrush::GetEndPoint](#getendpoint)|检索线性渐变的结束坐标|
|[CD2DLinearGradientBrush::GetStartPoint](#getstartpoint)|检索线性渐变的起始坐标|
|[CD2DLinearGradientBrush::SetEndPoint](#setendpoint)|线性渐变画笔的坐标空间中的终止坐标集|
|[CD2DLinearGradientBrush::SetStartPoint](#setstartpoint)|线性渐变画笔的坐标空间中的起始坐标设置|

### <a name="public-operators"></a>公共运算符

|名称|描述|
|----------|-----------------|
|[CD2DLinearGradientBrush::operator ID2D1LinearGradientBrush *](#operator_id2d1lineargradientbrush_star)|返回 ID2D1LinearGradientBrush 接口|

### <a name="protected-data-members"></a>受保护的数据成员

|name|描述|
|----------|-----------------|
|[CD2DLinearGradientBrush::m_LinearGradientBrushProperties](#m_lineargradientbrushproperties)|起点和终点的渐变。|
|[CD2DLinearGradientBrush::m_pLinearGradientBrush](#m_plineargradientbrush)|指向 ID2D1LinearGradientBrush 的指针。|

## <a name="inheritance-hierarchy"></a>继承层次结构

[CObject](../../mfc/reference/cobject-class.md)

[CD2DResource](../../mfc/reference/cd2dresource-class.md)

[CD2DBrush](../../mfc/reference/cd2dbrush-class.md)

[CD2DGradientBrush](../../mfc/reference/cd2dgradientbrush-class.md)

`CD2DLinearGradientBrush`

## <a name="requirements"></a>要求

**标头：** afxrendertarget.h

##  <a name="_dtorcd2dlineargradientbrush"></a>  CD2DLinearGradientBrush:: ~ CD2DLinearGradientBrush

析构函数。 当 D2D 线性渐变画笔对象被销毁时调用。

```
virtual ~CD2DLinearGradientBrush();
```

##  <a name="attach"></a>  CD2DLinearGradientBrush::Attach

附加现有的资源的对象的接口

```
void Attach(ID2D1LinearGradientBrush* pResource);
```

### <a name="parameters"></a>参数

*pResource*<br/>
现有资源的接口。 不能为 NULL

##  <a name="cd2dlineargradientbrush"></a>  CD2DLinearGradientBrush::CD2DLinearGradientBrush

构造一个 CD2DLinearGradientBrush 对象。

```
CD2DLinearGradientBrush(
    CRenderTarget* pParentTarget,
    const D2D1_GRADIENT_STOP* gradientStops,
    UINT gradientStopsCount,
    D2D1_LINEAR_GRADIENT_BRUSH_PROPERTIES LinearGradientBrushProperties,
    D2D1_GAMMA colorInterpolationGamma = D2D1_GAMMA_2_2,
    D2D1_EXTEND_MODE extendMode = D2D1_EXTEND_MODE_CLAMP,
    CD2DBrushProperties* pBrushProperties = NULL,
    BOOL bAutoDestroy = TRUE);
```

### <a name="parameters"></a>参数

*pParentTarget*<br/>
指向该呈现器目标的指针。

*gradientStops*<br/>
指向 D2D1_GRADIENT_STOP 结构数组的指针。

*gradientStopsCount*<br/>
值大于或等于 1，gradientStops 数组中指定的渐变停止点的数量。

*LinearGradientBrushProperties*<br/>
起点和终点的渐变。

*colorInterpolationGamma*<br/>
在哪种颜色执行内的插渐变停止点之间的空间。

*extendMode*<br/>
[0，1] 的规范化范围之外的渐变的行为。

*pBrushProperties*<br/>
一个指向不透明度和画笔的转换。

*bAutoDestroy*<br/>
指示所有者 (pParentTarget) 将销毁该对象。

##  <a name="create"></a>  CD2DLinearGradientBrush::Create

创建 CD2DLinearGradientBrush。

```
virtual HRESULT Create(CRenderTarget* pRenderTarget);
```

### <a name="parameters"></a>参数

*pRenderTarget*<br/>
指向该呈现器目标的指针。

### <a name="return-value"></a>返回值

如果该方法成功，它会返回 S_OK。 否则，它返回一个 HRESULT 错误代码。

##  <a name="destroy"></a>  CD2DLinearGradientBrush::Destroy

销毁 CD2DLinearGradientBrush 对象。

```
virtual void Destroy();
```

##  <a name="detach"></a>  CD2DLinearGradientBrush::Detach

分离对象中的资源接口

```
ID2D1LinearGradientBrush* Detach();
```

### <a name="return-value"></a>返回值

指向已分离的资源接口指针。

##  <a name="get"></a>  CD2DLinearGradientBrush::Get

返回 ID2D1LinearGradientBrush 接口

```
ID2D1LinearGradientBrush* Get();
```

### <a name="return-value"></a>返回值

指向 ID2D1LinearGradientBrush 接口或如果对象尚未初始化，则为 NULL 指针。

##  <a name="getendpoint"></a>  CD2DLinearGradientBrush::GetEndPoint

检索线性渐变的结束坐标

```
CD2DPointF GetEndPoint() const;
```

### <a name="return-value"></a>返回值

画笔的坐标空间中的线性渐变的二维终止坐标

##  <a name="getstartpoint"></a>  CD2DLinearGradientBrush::GetStartPoint

检索线性渐变的起始坐标

```
CD2DPointF GetStartPoint() const;
```

### <a name="return-value"></a>返回值

画笔的坐标空间中的线性渐变的二维起始坐标

##  <a name="m_lineargradientbrushproperties"></a>  CD2DLinearGradientBrush::m_LinearGradientBrushProperties

起点和终点的渐变。

```
D2D1_LINEAR_GRADIENT_BRUSH_PROPERTIES m_LinearGradientBrushProperties;
```

##  <a name="m_plineargradientbrush"></a>  CD2DLinearGradientBrush::m_pLinearGradientBrush

指向 ID2D1LinearGradientBrush 的指针。

```
ID2D1LinearGradientBrush* m_pLinearGradientBrush;
```

##  <a name="operator_id2d1lineargradientbrush_star"></a>  CD2DLinearGradientBrush::operator ID2D1LinearGradientBrush *

返回 ID2D1LinearGradientBrush 接口

```
operator ID2D1LinearGradientBrush*();
```

### <a name="return-value"></a>返回值

指向 ID2D1LinearGradientBrush 接口或如果对象尚未初始化，则为 NULL 指针。

##  <a name="setendpoint"></a>  CD2DLinearGradientBrush::SetEndPoint

线性渐变画笔的坐标空间中的终止坐标集

```
void SetEndPoint(CD2DPointF point);
```

### <a name="parameters"></a>参数

*点*<br/>
画笔的坐标空间中的线性渐变的二维终止坐标

##  <a name="setstartpoint"></a>  CD2DLinearGradientBrush::SetStartPoint

线性渐变画笔的坐标空间中的起始坐标设置

```
void SetStartPoint(CD2DPointF point);
```

### <a name="parameters"></a>参数

*点*<br/>
画笔的坐标空间中的线性渐变的二维起始坐标

## <a name="see-also"></a>请参阅

[类](../../mfc/reference/mfc-classes.md)
