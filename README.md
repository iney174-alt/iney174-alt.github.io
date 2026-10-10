# Hermes Personal Assistant — OAuth pages

Публичные статические страницы личного Telegram-ассистента: главная и политика конфиденциальности.

- Главная: https://iney174-alt.github.io/
- Политика конфиденциальности: https://iney174-alt.github.io/privacy.html

## GitHub Pages

1. В репозитории откройте **Settings → Pages**.
2. В **Build and deployment** выберите **Deploy from a branch**.
3. Выберите ветку **main**, папку **/ (root)** и нажмите **Save**.
4. Дождитесь публикации и проверьте ссылки выше.

## Google OAuth

1. В Search Console добавьте URL-prefix property `https://iney174-alt.github.io/` и подтвердите владение способом HTML file. Файл Google verification должен оставаться в корне сайта.
2. В Google Cloud OAuth branding укажите:
   - Home page: `https://iney174-alt.github.io/`
   - Privacy policy: `https://iney174-alt.github.io/privacy.html`
   - Authorized domain: `iney174-alt.github.io`
3. Сохраните изменения и проверьте, разрешает ли Google домен и публикацию приложения.

Приложение предназначено для личного использования. Статус Production избавляет внешний OAuth app от семидневного срока refresh token, который действует для External app в Testing. После смены статуса потребуется заново авторизовать аккаунт, если прежний refresh token уже отозван/истёк. Google может показывать предупреждение о непроверенном приложении и ограничивает количество пользователей.

Не добавляйте в этот репозиторий OAuth credentials, токены, данные Google или конфигурацию сервера.

Текст политики должен соответствовать фактической настройке Telegram-бота и подключённых сервисов обработки запросов.
