# ChatBot AI (React + Vite) — готовый проект

## Локально
1. Склонируй репозиторий или распакуй архив
2. Установи зависимости:
   ```bash
   npm install
   ```
3. Запуск:
   ```bash
   npm run dev
   ```
4. Открой http://localhost:5173

> Серверный эндпоинт `/api/chat` использует переменную окружения `OPENAI_API_KEY`. Локально можно использовать `vercel dev` или настроить dev-среду для работы функций.

## Деплой (рекомендую Vercel)
1. Создай репозиторий на GitHub и запушь код.
2. На vercel.com → New Project → Import GitHub Repo.
3. В проекте Vercel -> Settings -> Environment Variables добавить:
   - `OPENAI_API_KEY` = твой ключ OpenAI
4. Deploy — Vercel автоматически развернёт фронт и serverless функцию `/api/chat`.
5. Готово — поделись ссылкой.

## Безопасность
- Никогда не помещай ключ OpenAI в фронтенд (например, в VITE_ переменные) — только в серверные env.
