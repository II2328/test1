# Учебный центр «ПрофЛиния» — лендинг программы

Статический сайт для программы обучения:

- **Курс:** Оператор автоматических и полуавтоматических станков и линий станков
- **Объём:** 144 часа
- **Стоимость:** 74 000 ₽

## Локальный запуск

Откройте файл `index.html` в браузере.

## Публикация на GitHub Pages

В репозитории добавлен workflow `.github/workflows/deploy-pages.yml`, который:

1. запускается при push в ветки `main`, `master` и `work`;
2. проверяет наличие `index.html` и `styles.css`;
3. публикует содержимое репозитория как статический сайт на GitHub Pages.

### Важные настройки репозитория

1. `Settings` → `Pages`.
2. В разделе **Build and deployment** выбрать **Source: GitHub Actions**.
3. После push дождаться успешного выполнения workflow **Deploy static site to GitHub Pages**.

## Если видите 404

Проверьте, что открываете корректный URL:

- для **user/organization site** (репозиторий `username.github.io`):
  - `https://username.github.io/`
- для **project site** (обычный репозиторий):
  - `https://username.github.io/repository-name/`

Также добавлен `404.html`, который автоматически перенаправляет на главную страницу сайта.
