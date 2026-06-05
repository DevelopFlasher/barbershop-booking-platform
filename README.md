# Платформа записи в барбершоп

Веб-приложение для записи клиентов в барбершоп. Проект сделан как классическое Spring Boot MVC-приложение с регистрацией пользователей, авторизацией, ролями, административным разделом и хранением данных в PostgreSQL.

## Стек

- Java 17
- Spring Boot 2.6
- Spring Security
- Thymeleaf
- Spring Data JPA
- PostgreSQL
- Maven

## Возможности

- Регистрация и вход пользователей
- Запись клиента на услугу
- Просмотр записей пользователя
- Административная страница со списком клиентских записей
- Серверный HTML-интерфейс на Thymeleaf
- Настройка подключения к БД через переменные окружения

## Запуск

Создайте базу PostgreSQL и при необходимости задайте переменные из `.env.example`.

Linux/macOS:

```bash
./mvnw spring-boot:run
```

Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

## Конфигурация

| Переменная | Значение по умолчанию |
| --- | --- |
| `DATABASE_URL` | `jdbc:postgresql://localhost:5432/barbershop` |
| `DATABASE_USERNAME` | `postgres` |
| `DATABASE_PASSWORD` | `postgres` |

## Структура

```text
src/main/java/.../config       настройки безопасности
src/main/java/.../model        модели домена
src/main/java/.../repository   доступ к данным
src/main/java/.../service      бизнес-логика
src/main/java/.../web          MVC-контроллеры
src/main/resources/templates   Thymeleaf-шаблоны
src/main/resources/static      стили и изображения
```

## Для портфолио

Проект показывает базовую архитектуру монолитного Java web-приложения: MVC, Spring Security, JPA, шаблоны, формы и PostgreSQL.

