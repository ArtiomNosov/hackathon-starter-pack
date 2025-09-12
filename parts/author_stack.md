# 👨‍💻 Пример стека для хакатонов

## 🎯 Почему именно этот стек

**Принципы выбора:**
- **Скорость разработки** — быстро создать MVP
- **Знакомые технологии** — не тратить время на изучение
- **Простота деплоя** — легко задеплоить и показать
- **Готовые решения** — много библиотек и компонентов

## 🛠️ Инструменты разработки

### VS Code + расширения
**Расширения:**
- **ES7+ React/Redux/React-Native snippets**
- **Tailwind CSS IntelliSense**
- **Prisma** — подсветка синтаксиса
- **GitLens** — улучшенная работа с Git
- **Prettier** — форматирование кода

### Git + GitHub
- **GitHub** — хостинг кода
- **GitHub Actions** — CI/CD
- **Conventional Commits** — структурированные коммиты

## 🚀 CI/CD

### GitHub Actions
```yaml
name: Deploy
on:
  push:
    branches: [main]

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
      - run: npm ci
      - run: npm run build
      - uses: amondnet/vercel-action@v20
```

---

**Помните:** Это мой личный выбор. Выбирайте то, что знаете и что подходит вашей команде! 🚀
