# Chinese Premium Fashion — интернет-магазин на React

[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![React Router](https://img.shields.io/badge/React%20Router-7-CA4245?logo=reactrouter&logoColor=white)](https://reactrouter.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)

Одностраничное приложение (SPA) интернет-магазина премиальной одежды с восточной эстетикой. Реализовано на **React** с маршрутизацией через **React Router** и управлением корзиной через **Context API**.

## Возможности

- 🛍️ **Каталог** товаров с фильтрацией по категориям (`CategoryFilter`).
- 🔎 **Страница товара** с размерами, цветами, описанием и характеристиками.
- 🛒 **Корзина** на Context API (`CartContext`) — добавление, изменение количества, удаление.
- 📄 Страницы **Home, Catalog, Product Detail, About, Contact, Cart**.
- ⏳ Индикатор загрузки (`LoadingSpinner`), карточки товаров (`ProductCard`), общий Header/Footer.

## Маршруты

| Путь | Страница |
|------|----------|
| `/` | Главная |
| `/catalog` | Каталог |
| `/product/:id` | Карточка товара |
| `/cart` | Корзина |
| `/about` · `/contact` | О магазине · Контакты |

## Структура

```
src/
├── App.js                 # маршрутизация + CartProvider
├── context/CartContext.js # состояние корзины (Context API)
├── data/                  # products.js, categories.js — данные каталога
├── components/            # Header, Footer, ProductCard, CategoryFilter, LoadingSpinner
└── pages/                 # Home, Catalog, ProductDetail, About, Contact, Cart
```

## Запуск

```bash
git clone https://github.com/DenisDrobyshev/store.git
cd store
npm install
npm start        # http://localhost:3000
npm run build    # production-сборка
```

## Стек

`React 19` · `React Router 7` · `Context API` · `Create React App` · `CSS`
