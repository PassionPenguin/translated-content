---
title: <xsl:when>
slug: Web/XML/XSLT/Reference/Element/when
l10n:
  sourceCommit: 3e1b5277c6451e7d27ab628f23fb9702947a7a7b
---

`<xsl:when>` 要素は `<xsl:choose>` 要素内に常に表示され、case 文のように動作します。

### 構文

```xml
<xsl:when test=EXPRESSION>
  TEMPLATE
</xsl:when>
```

### 必須属性

- `test`
  - : 評価される論理式を指定します。true の場合、要素の内容が処理されます。false の場合は無視されます。

### 任意属性

なし。

### 種類

サブ命令で、常に `<xsl:choose>` 要素内に現れます。

## 仕様書

XSLT, section 9.2.

## Gecko の対応

対応済み。
