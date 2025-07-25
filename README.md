# swagger-petstore-api-testing
# 🧪 API Testing Project: Swagger Petstore

## 📌 Описание
Ручное тестирование REST API на примере Swagger Petstore: https://petstore.swagger.io/  
Цель: выявить ошибки в логике работы, проверить корректность ответов сервера, валидировать поведение на граничных значениях.

## 🧰 Используемые инструменты
- **Postman** (v 11.53.0)
- **Swagger UI**
- **Windows 10 Pro + Google Chrome**
- Документация: PDF-файлы с тест-кейсами и баг-репортами
- GitHub — для хранения артефактов тестирования

## 📝 Что протестировано
- **Поиск питомцев** по статусам и ID
- **Добавление, изменение, удаление** питомцев
- **Работа с заказами** (POST, GET, DELETE)
- **Аутентификация и работа с пользователями**
- Обработка **ошибочных входных данных**

## ✅ Покрытие
- 30+ тест-кейсов, включая позитивные и негативные сценарии
- 3 критичных и средних баг-репорта
- Примеры неправильного поведения API (например, 200 OK при ошибках)

## 📄 Документация
- 📋 [Тест-кейсы](https://github.com/Irina-Arma/swagger-petstore-api-testing/blob/34d8882b604c8eab1ddbbb41650b8198bc4b92d8/docs/TestCases_Swagger%20Petstore.pdf)
- 🐞 [Баг-репорты](https://github.com/Irina-Arma/swagger-petstore-api-testing/blob/4acfc018db38f50e593c5e99486a79485a6ef62b/docs/BugReports_Swagger%20Petstore.pdf)


## 🐞 Найденные баги
| ID      | Описание                                                                 | Критичность | Приоритет |
|---------|--------------------------------------------------------------------------|-------------|------------|
| Bug-001 | 200 OK при запросе с несуществующим статусом вместо 404                 | Minor       | Medium     |
| Bug-002 | Можно создать заказ с неверным типом данных (complete ≠ boolean)        | Major       | High       |
| Bug-003 | API авторизует несуществующего пользователя (200 OK вместо 404)         | Critical    | High       |

📄 Полные баг-репорты: [`BugReports_SwaggerPetstore.pdf`](https://github.com/Irina-Arma/swagger-petstore-api-testing/blob/4acfc018db38f50e593c5e99486a79485a6ef62b/docs/BugReports_Swagger%20Petstore.pdf)

## 📄 Тест-кейсы
Содержат:
- Полные шаги воспроизведения
- Ожидаемый и фактический результат
- Статус (Passed / Failed)
- Ссылки на соответствующие баги

📄 Документ: [`TestCases_SwaggerPetstore.pdf`](https://github.com/Irina-Arma/swagger-petstore-api-testing/blob/34d8882b604c8eab1ddbbb41650b8198bc4b92d8/docs/TestCases_Swagger%20Petstore.pdf)

## 💼 Навыки, продемонстрированные в проекте
- Проектирование тест-кейсов по API
- Анализ спецификаций и валидация ответов
- Написание баг-репортов
- Использование Postman

## 🔄 Коллекции Postman
В директории [`postman/`](postman) находятся экспортированные коллекции и окружения:
- [Swagger Petstore.postman_collection.json](https://github.com/Irina-Arma/swagger-petstore-api-testing/blob/26ca493f0a0f1b5ec1d8139d243fcc68464a94e3/postman/Swagger%20Petstore.postman_collection.json) — основной набор запросов
