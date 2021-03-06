---
title: OpenMP 库
ms.date: 10/24/2018
ms.assetid: f89abf97-67e3-4327-bc30-43f85b9533a2
ms.openlocfilehash: 75f772c953a2120a02f72d8bdfc73c1baaaef390
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50530333"
---
# <a name="openmp-libraries"></a>OpenMP 库

讨论组成 Visual c + + OpenMP 运行时库的.lib 文件。

以下库包含 Visual c + + OpenMP 运行时库函数。

|OpenMP 运行时库|特征|
|------------------------------|---------------------|
|VCOMP.LIB|多线程、 动态链接 （VCOMP 导入库。LIB)。|
|VCOMPD.LIB|多线程、 动态链接 （VCOMPD 导入库。合上盖子） （调试）|

如果在编译时定义 _DEBUG 并且如果`#include omp.h`是源代码，VCOMPD 中。LIB 将默认 lib。 否则为 VCOMP。将使用 LIB。

可以使用[/NODEFAULTLIB （忽略库）](../../../build/reference/nodefaultlib-ignore-libraries.md)若要删除默认 lib 并显式链接到与所选的库。

OpenMP Dll Visual c + + 可再发行组件目录中，需要随使用 OpenMP 的应用程序一起分发。

## <a name="see-also"></a>请参阅

[库参考](openmp-library-reference.md)
