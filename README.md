# SIGNAL IN — Событийный радар

Публичная статическая страница архитектуры MVP «Событийного радара».

**Сайт:** https://mvlbulankin.github.io/t-ai-contest/

## Локальный просмотр

```bash
python3 -m http.server 8000 --directory docs
```

Открыть http://localhost:8000/.

## Сборка CSS

Требуется Node.js 24:

```bash
npm ci
npm run build:css
```

Для автоматической пересборки при редактировании:

```bash
npm run watch:css
```

## Деплой

GitHub Pages публикуется через `.github/workflows/pages.yml` после push в `main`. В публичный артефакт входят только `index.html` и собранный `styles.css`.

Репозиторий намеренно содержит только лендинг и его tooling. Остальные материалы проекта хранятся локально и исключены через `.gitignore`.
