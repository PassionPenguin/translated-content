---
title: ::backdrop
slug: Web/CSS/::backdrop
---

{{CSSRef}}

[CSS](/ru/docs/Web/CSS) [псевдо-элемент](/ru/docs/Web/CSS/Pseudo-elements) **`::backdrop`** это прямоугольник с размерами {{Glossary("viewport", "окна")}}, который отрисовывается сразу же после отрисовки любого элемента в полноэкранном режиме. Это включает элементы, установленные в полноэкранный режим с помощью [Fullscreen API](/ru/docs/Web/API/Fullscreen_API) и элементы {{HTMLElement("dialog")}}.

Когда несколько элементов находятся в полноэкранном режиме, подложка появляется под тем из них, который находится на переднем плане и над всеми остальными.

```css
/* Подложка показывается только тогда, когда диалоговое окно открыто с помощью метода dialog.showModal() */
dialog::backdrop {
  background: rgba(255, 0, 0, 0.25);
}
```

Все полноэкранные элементы появляются в порядке last-in/first out (LIFO - последним пришёл - первым ушёл) на специальном верхнем слое окна, который всегда отрисовывается последним (поэтому поверх остальных) до отрисовки содержимого окна. Псевдо-элемент `::backdrop` позволяет затемнить, стилизовать или полностью спрятать всё, что находится под элементом, когда он находится на этом верхнем слое.

`::backdrop` не наследует от других элементов и другие элементы не могут от него наследовать. Нет никаких ограничений на свойства, которые можно применять к этому псевдо-элементу.

## Синтаксис

{{CSSSyntax}}

## Примеры

В этом примере, стиль подложки при открытии видео в полноэкранном режиме делаёт её серо-голубой, а не серой, какой она является по стандарту в большинстве браузеров.

```css
video::backdrop {
  background-color: #448;
}
```

В результате окно выглядит так:

![](bbb-backdrop.png)

Обратите внимание на эффект серо-голубых полей сверху и снизу, где подложка видна. Обычно эта область чёрная, но её цвет изменён с помощью CSS кода выше.

## Спецификации

{{Specifications}}

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- {{cssxref(":fullscreen")}} псевдокласс
- {{HTMLElement("dialog")}} HTML-элемент
- [Fullscreen API](/ru/docs/Web/API/Fullscreen_API)
