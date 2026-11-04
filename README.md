# Abacadabra — лендінг

Статичний сайт (HTML + CSS + JS), без збірки й бібліотек. Працює на GitHub Pages.

## Структура
```
index.html        — вхід: веде на /uk/ (або /en/ для англомовного браузера)
uk/index.html     — українська версія (основна)
en/index.html     — англійська версія
privacy.html      — політика конфіденційності (UA + EN, шаблон)
terms.html        — умови та повернення (UA + EN, шаблон)
assets/style.css  — стилі
assets/main.js    — меню, абакус, перемикач тарифу, форма, cookie-банер
assets/favicon.svg, assets/og-image.png
robots.txt, sitemap.xml, .nojekyll
```

## Публікація на GitHub Pages
1. github.com → **New repository** (наприклад, `abacadabra`), Public.
2. **Add file → Upload files** → перетягніть **вміст** розпакованого архіву (файли й папки `uk`, `en`, `assets`) → **Commit changes**.
3. **Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save**.
4. Через 1–2 хв сайт відкриється за адресою `https://ВАШ-ЛОГІН.github.io/abacadabra/`.
5. Власний домен: **Settings → Pages → Custom domain** + запис DNS у реєстратора (GitHub покаже інструкцію).

## Що замінити (пошук і заміна в усіх файлах)
| Шукати | Замінити на |
|---|---|
| `https://example.com` | ваш домен або `https://ВАШ-ЛОГІН.github.io/abacadabra` — у .html, robots.txt, sitemap.xml |
| `YOUR_FORM_ID` | ID форми Formspree (нижче) — в `uk/` і `en/` |
| `YOUR_BOOKING_LINK` | посилання Cal.com / Calendly на 20-хв знайомство |
| `YOUR_NUMBER` | номер WhatsApp без «+» і пробілів (напр. `380501234567`) |
| `YOUR_USERNAME` | нік Telegram |
| `YOUR_EMAIL`, `YOUR_INSTAGRAM` | контакти бренду |
| `[ІМ'Я…]`, `[Кваліфікація…]` | дані викладачки — лише підтверджені факти |
| `[уточнити з викладачкою]`, `[після погодження]` | коментарі/тексти, які треба погодити |
| `[дужки]` у privacy.html і terms.html | ваші дані та умови; показати юристу |

## Форма і календар (безкоштовно)
1. **Formspree:** formspree.io → New form → вкажіть email для заявок → скопіюйте код із адреси `https://formspree.io/f/abcdwxyz` → замініть `YOUR_FORM_ID` на `abcdwxyz`.
2. **Календар:** cal.com або calendly.com → подія «Знайомство 20 хв» → скопіюйте посилання → замініть `YOUR_BOOKING_LINK`. Після заявки сайт сам перекине батьків у календар.
3. Поки форма не підключена, сайт просить написати в месенджер — нічого не ламається.

## Фото
- Додайте файли в `assets/` у форматі WebP (до ~150 КБ).
- У HTML поруч із кожним плейсхолдером є закоментований тег `<img …>` з alt-текстом — розкоментуйте його і видаліть плейсхолдер.
- Фото дітей — лише з письмовою згодою батьків.

## Відгуки
Блок 11 закоментований в `uk/index.html`. Розкоментуйте після пілоту: текст + ім'я мами + країна + вік дитини, лише зі згодою.

## Після запуску
- Google Search Console → додайте сайт → надішліть `sitemap.xml`.
- Перевірте розмітку: https://validator.schema.org і https://search.google.com/test/rich-results
- Видимість в AI-асистентах не гарантована: вона залежить від якості контенту, зовнішніх згадок і алгоритмів платформ.
