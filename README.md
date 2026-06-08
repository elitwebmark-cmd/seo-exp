# elit-web · SEO-експеримент

Інтерактивна інфографіка результатів SEO-експерименту для elit-web.ua. Аналіз позицій 482 запитів у Google.com.ua (Київ) на 5 датах: старт → 19.05.2026 → 26.05.2026 → 01.06.2026 → 08.06.2026.

## Локальний запуск

```bash
npm install
npm start
```

Сторінка буде доступна на http://localhost:3000.

## Деплой на Railway

1. Запуш цей репозиторій на GitHub.
2. Зайди на [railway.com](https://railway.com), створи новий проект → **Deploy from GitHub repo** → обери цей репозиторій.
3. Railway автоматично визначить Node.js, виконає `npm install` і запустить `npm start`.
4. У налаштуваннях проекту → Settings → Networking → **Generate Domain** — отримаєш публічну URL.

Усі залежності фронтенду (Chart.js, шрифт Mulish) підвантажуються з CDN — додаткових налаштувань не потрібно.

## Структура

- `index.html` — увесь дешборд (HTML + CSS + JS + дані) в одному файлі
- `package.json` — мінімальний Node-сервер (пакет `serve`) для роздачі статики
- `.gitignore` — виключає `node_modules`

## Технології

- HTML5 + CSS3 (Mulish font, кастомний дизайн)
- Chart.js 4.5.0 (через CDN)
- Vanilla JavaScript (без фреймворків)
- Node.js + serve (для прод-роздачі)
