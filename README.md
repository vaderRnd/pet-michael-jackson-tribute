# Michael Jackson Tribute

Лендинг-трибьют, посвящённый творчеству Майкла Джексона. Написан на чистом HTML и CSS с подходом mobile-first.

## Демо

Откройте `index.html` в браузере.

## Структура проекта

```
├── index.html
├── css/
│   ├── main.css              # Точка входа, импортирует все стили
│   ├── normalize.css         # Сброс стилей браузера
│   ├── vars.css              # CSS-переменные и базовые стили
│   └── components/
│       ├── header.css
│       ├── hero.css
│       ├── discography.css
│       └── footer.css
└── img/
    ├── mj-portrait-compressed.jpg
    ├── cover/                # Обложки альбомов
    └── concert/              # Фото концертов
```

## Секции страницы

| Секция | Якорь | Описание |
|---|---|---|
| Главная | `#home` | Hero с портретом и CTA |
| Дискография | `#discography` | 6 альбомов (1979–2001) |
| О легенде | `#about` | Биография |
| Галерея | `#gallery` | Концертные фото |

## CSS-переменные

Определены в `css/vars.css`:

```css
--primary-color: #000000
--accent-color:  #ffd700
--text-color:    #333333
--bg-color:      #ffffff
--bg-secondary:  #f5f5f5
--container-width: 1200px
--header-height: 70px
```

## Особенности

- Подход **mobile-first** — стили пишутся для мобильных, затем расширяются через media queries
- Адаптивная вёрстка под разные устройства
- Бургер-меню на мобильных (реализовано через CSS checkbox hack, без JS)
- Lazy loading изображений (`loading="lazy"`)
- Фиксированный header с якорной навигацией
- Семантическая разметка (`header`, `main`, `section`, `article`, `footer`)
- Open Graph мета-теги
