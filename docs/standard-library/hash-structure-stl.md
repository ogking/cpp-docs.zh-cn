---
title: hash 结构（C++ 标准库）| Microsoft Docs
ms.date: 11/04/2016
f1_keywords:
- thread/std::hash
ms.assetid: 4a8bf5bc-4334-4070-936b-98585f8a073b
ms.openlocfilehash: bb230d401d5061f4951f8007f93c3a28ce3dab03
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50579853"
---
# <a name="hash-structure-c-standard-library"></a>hash 结构（C++ 标准库）

定义一个成员函数，该函数返回一个由 `Val` 唯一决定的值。 此成员函数定义一个 [hash](../standard-library/hash-class.md) 函数，此函数适用于将 `thread::id` 类型的值映射到索引值的分布。

## <a name="syntax"></a>语法

```cpp
template <>
struct hash<thread::id> :
    public unary_function<thread::id, size_t>
{
    size_t operator()(thread::id Val) const;

};
```

## <a name="requirements"></a>要求

**标头：** \<线程 >

**命名空间：** std

## <a name="see-also"></a>请参阅

[头文件引用](../standard-library/cpp-standard-library-header-files.md)<br/>
[\<thread>](../standard-library/thread.md)<br/>
[unary_function 结构](../standard-library/unary-function-struct.md)<br/>
