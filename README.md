# Ферма Пузырей

HTML5-игра (аркада / головоломка «собери группу») для **VK Mini Apps / VK Games**.

- **App ID:** `54692985`
- **Платформы:** Web, m.vk, Android, iOS
- **Версия:** 1.1

## URL для dev.vk.ru (GitHub Pages)

После пуша в `main` сайт публикуется автоматически:

| | |
|---|---|
| **Игра** | https://puma04121990-blip.github.io/ferma-puzyrey/ |
| **index** | https://puma04121990-blip.github.io/ferma-puzyrey/index.html |
| **ПС** | https://puma04121990-blip.github.io/ferma-puzyrey/terms.html |
| **Политика** | https://puma04121990-blip.github.io/ferma-puzyrey/privacy.html |

### Куда вставить в [dev.vk.ru](https://dev.vk.ru)

**Настройки приложения → URL / Хостинг / Площадки** (названия могут отличаться):

| Платформа | URL |
|-----------|-----|
| Web (iframe) | `https://puma04121990-blip.github.io/ferma-puzyrey/` |
| Mobile (iOS / Android) | `https://puma04121990-blip.github.io/ferma-puzyrey/` |
| m.vk | `https://puma04121990-blip.github.io/ferma-puzyrey/` |

Запуск в клиенте: https://vk.ru/app54692985

> Важно: в кабинете должен быть указан **HTTPS-URL игры** (Pages), а не страница README репозитория.

## Структура

```
build/                 # то, что уходит на GitHub Pages
  index.html
  privacy.html
  terms.html
  *.png, vk-bridge.min.js
.github/workflows/     # автодеплой Pages
package.json           # vk-miniapps-deploy (опционально, если нужен VK Hosting)
vk-hosting-config.json
```

## Локальный запуск

1. Откройте папку `build` в VS Code.
2. Live Server → `build/index.html`  
   или: http://127.0.0.1:5500/

Вне клиента ВКонтакте игра работает в **локальном режиме** (без облака/рекламы VK).

## Обновление сайта

```bash
git add .
git commit -m "update"
git push origin main
```

Через 1–2 минуты после зелёного Actions обновится  
https://puma04121990-blip.github.io/ferma-puzyrey/

## VK Hosting (альтернатива, не обязателен)

```bash
npm install
npm run deploy
```

Нужен доступ администратора приложения в [dev.vk.ru](https://dev.vk.ru).

## Документы

- Пользовательское соглашение: `build/terms.html`
- Политика конфиденциальности: `build/privacy.html`
