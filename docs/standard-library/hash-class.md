---
title: hash 类
ms.date: 11/04/2016
f1_keywords:
- functional/std::hash
- bitset/std::hash
- memory/std::hash
- string/std::hash
- system_error/std::hash
- thread/std::hash
- typeindex/std::hash
- vector/std::hash
- XSTDDEF/std::hash
- xstring/std::hash
helpviewer_keywords:
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
- std::hash [C++]
ms.assetid: e1b500c6-a5c8-4f6f-ad33-7ec52eb8e2e4
ms.openlocfilehash: 2f7206e3764df384004b78e6df2127833a784f70
ms.sourcegitcommit: afd6fac7c519dbc47a4befaece14a919d4e0a8a2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2018
ms.locfileid: "51521021"
---
# <a name="hash-class"></a>hash 类

计算值的哈希代码。

## <a name="syntax"></a>语法

```cpp
template <class Ty>
struct hash {
    size_t operator()(Ty val) const;
};
```

## <a name="remarks"></a>备注

此成员对象定义一个哈希函数，适合将 Ty 类型的值映射到索引值的分布。 成员 `operator()` 会返回 *val* 的一个哈希代码，适合用于模板类 `unordered_map`、`unordered_multimap`、`unordered_set` 和 `unordered_multiset`。 此标准库对基本类型提供专用化：Ty 可能为任何标量类型，包括指针类型和枚举类型。 此外，还具有库类型 `string`、`wstring`、`u16string`、`u32string`、`string_view`、`wstring_view`、`u16string_view`、`u32string_view`、`bitset`、`error_code`、`error_condition`、`optional`、`shared_ptr`、`thread` `type_index`、`unique_ptr`、`variant` 和 `vector<bool>` 的专用化。

## <a name="example"></a>示例

```cpp
// std__functional__hash.cpp
// compile with: /EHsc
#include <functional>
#include <iostream>
#include <unordered_set>

int main()
    {
    std::unordered_set<int, std::hash<int> > c0;
    c0.insert(3);
    std::cout << *c0.find(3) << std::endl;

    return (0);
    }
```

```Output
3
```

## <a name="requirements"></a>要求

**标头：**\<functional>

**命名空间：** std

## <a name="see-also"></a>请参阅

[<unordered_map>](../standard-library/unordered-map.md)<br/>
[unordered_multimap 类](../standard-library/unordered-multimap-class.md)<br/>
[unordered_multiset 类](../standard-library/unordered-multiset-class.md)<br/>
[<unordered_set>](../standard-library/unordered-set.md)<br/>
