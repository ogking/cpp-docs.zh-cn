---
title: frexp、 frexpf、 frexpl
ms.date: 04/05/2018
apiname:
- frexp
apilocation:
- msvcrt.dll
- msvcr80.dll
- msvcr90.dll
- msvcr100.dll
- msvcr100_clr0400.dll
- msvcr110.dll
- msvcr110_clr0400.dll
- msvcr120.dll
- msvcr120_clr0400.dll
- ucrtbase.dll
- api-ms-win-crt-math-l1-1-0.dll
apitype: DLLExport
f1_keywords:
- frexp
- _frexpl
helpviewer_keywords:
- _frexpl function
- mantissas, floating-point variables
- frexpl function
- exponent, floating-point numbers
- frexp function
- floating-point functions, mantissa and exponent
ms.assetid: 9b020f2e-3967-45ec-a6a8-d467a071aa55
ms.openlocfilehash: c9e259f730d2d63d07032735be930f6f0fdb17e5
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50563834"
---
# <a name="frexp-frexpf-frexpl"></a>frexp、 frexpf、 frexpl

获取浮点数的尾数和指数。

## <a name="syntax"></a>语法

```C
double frexp(
   double x,
   int *expptr
);
float frexpf(
   float x,
   int * expptr
);
long double frexpl(
   long double x,
   int * expptr
);
float frexp(
   float x,
   int * expptr
);  // C++ only
long double frexp(
   long double x,
   int * expptr
);  // C++ only
```

### <a name="parameters"></a>参数

*x*<br/>
浮点值。

*expptr*<br/>
指向存储的整数指数的指针。

## <a name="return-value"></a>返回值

**frexp**返回表示尾数。 如果*x*为 0，则该函数返回 0 表示尾数和指数。 如果*expptr*是**NULL**，如中所述，将调用无效的参数处理程序[参数验证](../../c-runtime-library/parameter-validation.md)。 如果允许执行继续，此函数可设置**errno**到**EINVAL** ，并返回 0。

## <a name="remarks"></a>备注

**Frexp**函数将分解的浮点值 (*x*) 分解为一个尾数 (*m*) 和一个指数 (*n*)，这样，绝对值*m*大于或等于 0.5 且小于 1.0，并*x* = *m* * 2<sup>*n*</sup>. 整数指数*n*指向的位置处存储*expptr*。

C + + 允许重载，因此可以调用的重载**frexp**。 在 C 程序中， **frexp**始终采用**double**和一个**int**指针和返回**double**。

## <a name="requirements"></a>要求

|函数|必需的标头|
|--------------|---------------------|
|**frexp**， **frexpf**， **frexpl**|\<math.h>|

有关其他兼容性信息，请参阅 [兼容性](../../c-runtime-library/compatibility.md)。

## <a name="example"></a>示例

```C
// crt_frexp.c
// This program calculates frexp( 16.4, &n )
// then displays y and n.

#include <math.h>
#include <stdio.h>

int main( void )
{
   double x, y;
   int n;

   x = 16.4;
   y = frexp( x, &n );
   printf( "frexp( %f, &n ) = %f, n = %d\n", x, y, n );
}
```

```Output
frexp( 16.400000, &n ) = 0.512500, n = 5
```

## <a name="see-also"></a>请参阅

[浮点支持](../../c-runtime-library/floating-point-support.md)<br/>
[ldexp](ldexp.md)<br/>
[modf、modff、modfl](modf-modff-modfl.md)<br/>
