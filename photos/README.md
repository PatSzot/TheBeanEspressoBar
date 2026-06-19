# The Bean Espresso Bar — Photo Assets

All images optimized for web. Use WebP as primary source, JPEG as fallback.

## Files

| Slug | WebP | JPG | Dimensions | Best Use |
|------|------|-----|------------|----------|
| `espresso-pastries-window` | 65KB | 116KB | 1290×840 | Hero, About section — wide landscape shot of table with espresso cup, croissant, branded iced cup, street view through window |
| `iced-latte-logo` | 25KB | 51KB | 1290×836 | Brand moment — close-up of The Bean branded iced latte cup with logo visible, pastry bokeh background |
| `lifestyle-table-flatlay` | 63KB | 140KB | 1290×1280 | Lifestyle / mood — overhead flatlay of marble table with espresso, iced drink, sunglasses, silk scarf |
| `iced-latte-plants` | 52KB | 119KB | 1209×1400 | Menu section or gallery — portrait iced latte against tropical plant background |

## HTML Usage Pattern (with WebP + JPEG fallback)

```html
<picture>
  <source srcset="photos/espresso-pastries-window.webp" type="image/webp">
  <img src="photos/espresso-pastries-window.jpg"
       alt="Espresso, croissant and iced latte at a window table at The Bean Espresso Bar"
       width="1290" height="840"
       loading="lazy">
</picture>
```

Use `loading="eager"` on the hero image only. All others: `loading="lazy"`.

## Folder Structure for Site

```
/
├── index.html
└── photos/
    ├── espresso-pastries-window.webp   ← hero candidate
    ├── espresso-pastries-window.jpg
    ├── iced-latte-logo.webp            ← brand/about section
    ├── iced-latte-logo.jpg
    ├── lifestyle-table-flatlay.webp    ← mood / lifestyle
    ├── lifestyle-table-flatlay.jpg
    ├── iced-latte-plants.webp          ← menu or gallery
    └── iced-latte-plants.jpg
```
