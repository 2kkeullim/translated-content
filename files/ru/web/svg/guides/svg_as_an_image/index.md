---
title: SVG как изображение
slug: Web/SVG/Guides/SVG_as_an_image
---

{{SVGRef}}

Изображения SVG могут использоваться как формат изображения в ряде контекстов. Многие браузеры поддерживают изображения SVG:

- Элементы HTML {{HTMLElement("img")}} или {{SVGElement("svg")}}
- CSS {{cssxref("background-image")}}

## Гекко-специфические контексты

Кроме того, Gecko 2.0 представил поддержку использования [SVG](/ru/docs/Web/SVG) в следующих контекстах:

- CSS {{cssxref("list-style-image")}}
- CSS {{cssxref("content")}}
- Элементы SVG {{SVGElement("image")}}
- Элементы SVG {{SVGElement("feImage")}}
- Функция Canvas [`drawImage`](/ru/docs/HTML/Canvas/Tutorial/Using_images#drawImage)

### Ограничения

В целях безопасности, Gecko накладывает некоторые ограничения на контент SVG, когда он используется в качестве изображения:

- [JavaScript](/ru/docs/Web/JavaScript) отключён.
- Внешние ресурсы (например, изображения, таблицы стилей) не могут быть загружены, хотя их можно использовать, если они встроены в данные: URI.
- {{cssxref(":visited")}}-стили ссылок не отображаются.
- Стилизация виджитов на платформе (основанная на теме ОС) отключена.

Обратите внимание, что вышеуказанные ограничения являются специфическими для контекстов изображения; они не применяются, когда содержимое SVG просматривается напрямую или когда оно внедрено в виде документа с помощью встраивания элементов {{HTMLElement("iframe")}}, {{HTMLElement("object")}}, или {{HTMLElement("embed")}}.

## Спецификации

{{Specifications}}

## Смотрите также

- [SVG в HTML. Введение](/ru/docs/Web/SVG/Guides/SVG_in_HTML)
