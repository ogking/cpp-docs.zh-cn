---
title: 浮点协处理器和调用约定
ms.date: 11/04/2016
helpviewer_keywords:
- floating-point numbers [C++]
- floating-point coprocessor
ms.assetid: 3cc6615a-b308-4cf7-9570-83e192a832b3
ms.openlocfilehash: 7e9184d66bde26ab0e2b345f8f10c2e28619fd2b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50625103"
---
# <a name="floating-point-coprocessor-and-calling-conventions"></a>浮点协处理器和调用约定

如果你正在编写程序集的浮点例程点协处理器，则必须保留浮点控制字和清理协处理器堆栈，除非您在返回**float**或**double**值 （其中 st(0 应返回您的函数。

## <a name="see-also"></a>请参阅

[调用约定](../cpp/calling-conventions.md)