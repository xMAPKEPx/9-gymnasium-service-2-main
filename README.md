# Gymnasium Service

**Gymnasium Service** — это современное приложение для управления пользователями, реализованное на стеке React + TypeScript + Vite + Redux Toolkit + shadcn/ui.

## Описание

- Аутентификация и регистрация пользователей (mock/demo)
- Список пользователей и страница профиля
- Современный UI на shadcn/ui и TailwindCSS
- Моковые данные для демонстрации (без реального бэкенда)
- Защищённые маршруты (PrivateRoute)
- Уведомления через Sonner

## Стек технологий

- React 18+
- TypeScript
- Vite
- Redux Toolkit
- shadcn/ui (на базе TailwindCSS)
- React Router v6
- Sonner (уведомления)

## Структура проекта

```
src/
  api/                // Работа с API (axios-инстанс, сервисы)
  components/         // UI-компоненты (shadcn/ui, формы)
  const/              // Моковые константы (например, users.ts)
  pages/              // Страницы приложения (LoginPage, UsersPage, UserPage, RegisterPage)
  store/              // Redux Toolkit store, слайсы, хуки
  App.tsx             // Главный компонент приложения и роутинг
  main.tsx            // Точка входа
```

## Как запустить dev-сервер

1. Установите зависимости:
   ```bash
   npm install
   ```

2. Запустите dev-сервер:
   ```bash
   npm run dev
   ```

3. Откройте [http://localhost:5173](http://localhost:5173) в браузере.

## Основные возможности

- **Авторизация:** форма логина, проверка пароля, переход к списку пользователей.
- **Регистрация:** отдельная страница, валидация совпадения паролей.
- **Список пользователей:** карточки с аватаром, ролью, email, переход к профилю.
- **Профиль пользователя:** подробная информация, действия (редактировать, заблокировать и т.д.).
- **Защищённые маршруты:** доступ к /users и профилям только после авторизации.
- **Современный дизайн:** shadcn/ui, адаптивная верстка, уведомления.

## Примечания

- Для демонстрации используются моковые данные (см. `src/const/users.ts`).
- Для реальной интеграции с API потребуется доработать сервисы в `src/api/`.
- CORS и авторизация через cookie с внешними API (например, dummyjson.com) требуют прокси или собственного бэкенда.
