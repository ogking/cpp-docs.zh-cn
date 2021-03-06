---
title: 常量摘要
ms.date: 11/04/2016
helpviewer_keywords:
- constants, C
ms.assetid: 4158234c-e189-4e25-970f-52a04bc6380a
ms.openlocfilehash: 1da2a7434ced7f38fa199e5911e01709983fda91
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2018
ms.locfileid: "50547857"
---
# <a name="summary-of-constants"></a>常量摘要

常数：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;floating-point-constant<br/>
&nbsp;&nbsp;&nbsp;&nbsp;integer-constant<br/>
&nbsp;&nbsp;&nbsp;&nbsp;enumeration-constant<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*character-constant*

*floating-point-constant*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;fractional-constant exponent-part<sub>opt</sub> floating-suffix<sub>opt</sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;digit-sequence exponent-part floating-suffix<sub>opt</sub>

*fractional-constant*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;digit-sequence<sub>opt</sub> . *digit-sequence*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;digit-sequence  .

*exponent-part*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;e sign<sub>opt</sub> digit-sequence<br/>
&nbsp;&nbsp;&nbsp;&nbsp;E sign<sub>opt</sub> digit-sequence

*sign*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;+ -

*digit-sequence*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*digit*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;digit-sequence digit

*floating-suffix*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;f l F L

*integer-constant*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;decimal-constant integer-suffix<sub>opt</sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;binary-constant integer-suffix<sub>opt</sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;octal-constant integer-suffix<sub>opt</sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;hexadecimal-constant integer-suffix<sub>opt</sub>

*decimal-constant*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;nonzero-digit<br/>
&nbsp;&nbsp;&nbsp;&nbsp;decimal-constant digit

二进制常数：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0b binary-digit<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0B binary-digit

*octal-constant*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0<br/>
&nbsp;&nbsp;&nbsp;&nbsp;octal-constant octal-digit

*hexadecimal-constant*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0x  *hexadecimal-digit*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**0X**  *hexadecimal-digit*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;hexadecimal-constant hexadecimal-digit

*nonzero-digit*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;1 2 3 4 5 6 7 8 9

*octal-digit*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0 1 2 3 4 5 6 7

*hexadecimal-digit*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;0 1 2 3 4 5 6 7 8 9<br/>
&nbsp;&nbsp;&nbsp;&nbsp;a b c d e f<br/>
&nbsp;&nbsp;&nbsp;&nbsp;A B C D E F

*unsigned-suffix*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;u U

*long-suffix*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;l L

*character-constant*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;' c-char-sequence '<br/>
&nbsp;&nbsp;&nbsp;&nbsp;L' c-char-sequence '

*integer-suffix*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;unsigned-suffix long-suffix<sub>opt</sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;long-suffix unsigned-suffix<sub>opt</sub>

*c-char-sequence*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;c-char<br/>
&nbsp;&nbsp;&nbsp;&nbsp;c-char-sequence c-char

*c-char*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;除单引号 (**'**)、反斜杠 (**\\**) 或换行符 escape-sequence 以外的源字符集中的任何成员

*escape-sequence*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*simple-escape-sequence*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*octal-escape-sequence*<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*hexadecimal-escape-sequence*

*simple-escape-sequence*: one of<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**\a \b \f \n \r \t \v**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**\\' \\" \\\ \\?**

*octal-escape-sequence*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**\\ octal-digit**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;\\ octal-digit octal-digit<br/>
&nbsp;&nbsp;&nbsp;&nbsp;\\ octal-digit octal-digit octal-digit

*hexadecimal-escape-sequence*：<br/>
&nbsp;&nbsp;&nbsp;&nbsp;\x hexadecimal-digit<br/>
&nbsp;&nbsp;&nbsp;&nbsp;hexadecimal-escape-sequence hexadecimal-digit

## <a name="see-also"></a>请参阅

[词法语法](../c-language/lexical-grammar.md)<br/>
