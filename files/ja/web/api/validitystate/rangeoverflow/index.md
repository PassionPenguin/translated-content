---
title: ValidityState.rangeOverflow
slug: Web/API/ValidityState/rangeOverflow
l10n:
  sourceCommit: cfcbb39cc595bd536b107f6771bfb3f8e13bacca
---

{{APIRef("HTML DOM")}}

**`rangeOverflow`** は **[`ValidityState`](/ja/docs/Web/API/ValidityState)** オブジェクトの読み取り専用プロパティで、 {{HTMLElement("input")}} の値がユーザーに変更された後、その要素の [`max`](/ja/docs/Web/HTML/Reference/Attributes/max) 属性に設定された制約に適合しないことを示します。

フィールドが数値の性質を持つ場合、例えば {{HTMLElement("input/date", "date")}}, {{HTMLElement("input/month", "month")}}, {{HTMLElement("input/week", "week")}}, {{HTMLElement("input/time", "time")}}, {{HTMLElement("input/datetime-local", "datetime-local")}}, {{HTMLElement("input/number", "number")}}, {{HTMLElement("input/range", "range")}} の何れかの型であり、 `max` が設定されており、値が [`max`](/ja/docs/Web/HTML/Reference/Attributes/step) の値に設定された制約に適合しない場合、 `rangeOverflow` プロパティが true になります。

次のようになっていたとします。

```html
<input type="number" min="20" max="40" step="2" />
```

`value > 40` であれば、 `rangeOverflow` は true になります。 `true` の場合、その要素は CSS の {{cssxref(":invalid")}} および {{cssxref(":out-of-range")}} 擬似クラスに一致します。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{domxref("ValidityState.rangeUnderflow")}}
- [制約検証](/ja/docs/Web/HTML/Guides/Constraint_validation)
- [フォーム: データフォームの検証](/ja/docs/Learn_web_development/Extensions/Forms/Form_validation)
- [`step` 属性](/ja/docs/Web/HTML/Reference/Attributes/step)
- [`min` 属性](/ja/docs/Web/HTML/Reference/Attributes/min)
