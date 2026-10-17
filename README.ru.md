# Каталог кофе (Tel-Ran, 2023)

[English](README.md) | [Русский](README.ru.md)

Учебный проект на Java для управления каталогом кофе с помощью Spring Boot. Он объединяет серверные HTML-страницы, валидацию форм и работу с базой данных.

## Возможности и стек

- Просмотр, добавление, изменение, удаление и поиск записей о кофе.
- Отображение страниц через Thymeleaf и проверка данных форм.
- Работа с базой H2 в памяти через Spring Data JPA.
- Загрузка небольшого набора примеров кофе при старте.

В проекте используются Java 17 и Spring Boot 3.0.2. Контроллеры, сущности и репозитории находятся в [src/main/java/com/example/coffee](src/main/java/com/example/coffee), шаблоны страниц — в [src/main/resources/templates](src/main/resources/templates).

## Локальный запуск

Установите JDK 17 и Maven; команды `java` и `mvn` должны быть доступны в терминале.

```bash
git clone https://github.com/ivan-zamula/coffee-spring-boot-2023-tel-ran.git
cd coffee-spring-boot-2023-tel-ran
```

```bash
mvn spring-boot:run
```

Откройте [каталог](http://localhost:8080/coffees) в браузере. База H2 работает в памяти: изменения сохраняются на время текущего сеанса приложения. Параметры подключения находятся в [application.properties](src/main/resources/application.properties).
