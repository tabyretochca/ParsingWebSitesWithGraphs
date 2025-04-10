# Parsing Web Sites with Graphs

![Python](https://img.shields.io/badge/Python-3.12-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-0.95.2-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Описание проекта
**Parsing Web Sites with Graphs** — это веб-приложение, которое парсит веб-сайты, строит граф связей между страницами и предоставляет интерактивную визуализацию. Проект использует асинхронный парсинг с помощью `aiohttp`, обработку HTML через `BeautifulSoup`, построение графа с `networkx` и визуализацию через `pyvis`. Данные хранятся в Redis, а доступ предоставляется через REST API с авторизацией JWT.

Цель проекта — исследовать структуру сайтов и представить её в виде графа, где узлы — это страницы, а рёбра — ссылки между ними.

## Возможности
- Регистрация и аутентификация пользователей через JWT.
- Асинхронный парсинг сайтов с ограничением глубины и количества страниц.
- Построение направленного графа связей.
- Интерактивная визуализация графа в формате HTML.
- Кэширование результатов в Redis.

## Технологии
- **Backend**: FastAPI, SQLAlchemy, Alembic
- **Парсинг**: aiohttp, BeautifulSoup
- **Графы**: networkx, pyvis
- **Хранилище**: SQLite (база данных), Redis (кэш)
- **Аутентификация**: JWT (PyJWT)

## Установка
1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/<твой_username>/ParsingWebSitesWithGraphs.git
   cd ParsingWebSitesWithGraphs
