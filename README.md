# CSS Шпаргалка

Коллекция полезных CSS-отрезков с описаниями и примерами использования.

---

## Содержание

1. [Предотвращение дёргания страницы при прокрутке](#предотвращение-дёргания-страницы-при-прокрутке)
2. [Прозрачный статус-бар для PWA на iOS](#прозрачный-статус-бар-для-pwa-на-ios)

---

## Предотвращение дёргания страницы при прокрутке

Когда появляется модальное окно, страница может "дёргаться" из-за появления или исчезновения полосы прокрутки. Используйте свойство `scrollbar-gutter`, чтобы избежать этого.

### Пример кода:

```css
html {
  scrollbar-gutter: stable;
}
```

### Объяснение:
- **`scrollbar-gutter: stable;`**: Обеспечивает постоянное пространство для полосы прокрутки, предотвращая сдвиги макета.

[Документация MDN](https://developer.mozilla.org/ru/docs/Web/CSS/scrollbar-gutter)

---

## Прозрачный статус-бар для PWA на iOS

Чтобы создать бесшовный интерфейс для Progressive Web Apps (PWA) на iOS, можно сделать статус-бар прозрачным.

### Пример кода:

```html
<html lang="ru">
  <head>
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
  </head>
</html>
```

### Объяснение:
- **`content="black-translucent"`**: Включает полупрозрачный чёрный статус-бар, позволяя отображать фон PWA под ним.

[Документация Apple Developer](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html#//apple_ref/doc/uid/TP40008193-SW5)

---
