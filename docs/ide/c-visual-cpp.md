---
title: '&lt;c&gt; (Visual C++)'
ms.date: 11/04/2016
f1_keywords:
- <c>
helpviewer_keywords:
- <c> C++ XML tag
- c C++ XML tag
ms.assetid: 3b23fc0f-e10d-4dd0-b197-48a46cbddd9f
ms.openlocfilehash: 1efb411537e07ae9a5c2e4a70b5fa3ac319d79c3
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50431091"
---
# <a name="ltcgt-visual-c"></a>&lt;c&gt; (Visual C++)

\<c> 标记指示应将说明内的文本应标记为代码。 使用 [\<code>](../ide/code-visual-cpp.md) 指示作为代码的多行文本。

## <a name="syntax"></a>语法

```
<c>text</c>
```

#### <a name="parameters"></a>参数

*文本*<br/>
要指示为代码的文本。

## <a name="remarks"></a>备注

使用 [/doc](../build/reference/doc-process-documentation-comments-c-cpp.md) 进行编译可以将文档注释处理到文件中。

## <a name="example"></a>示例

```cpp
// xml_c_tag.cpp
// compile with: /doc /LD
// post-build command: xdcmake xml_c_tag.xdc

/// Text for class MyClass.
class MyClass {
public:
   int m_i;
   MyClass() : m_i(0) {}

   /// <summary><c>MyMethod</c> is a method in the <c>MyClass</c> class.
   /// </summary>
   int MyMethod(MyClass * a) {
      return a -> m_i;
   }
};
```

## <a name="see-also"></a>请参阅

[XML 文档](../ide/xml-documentation-visual-cpp.md)