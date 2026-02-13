## 📊 Полное тестирование API Reqres.in

Комплексное тестирование REST API сервиса [Reqres.in](https://reqres.in) с полным покрытием всех эндпоинтов и операций CRUD.
Инструмент тестирования: Postman

**Дата создания:** 4 декабря 2025  
**Количество запросов:** 14  
**Статус:** Завершено ✅

## Цели проекта
- ✅ 100% покрытие доступных эндпоинтов
- ✅ Тестирование позитивных и негативных сценариев
- ✅ Валидация структуры JSON-ответов
- ✅ Измерение производительности API
- ✅ Автоматизация тестовых проверок

## Ключевые результаты
| Метрика | Значение | Статус |
|---------|----------|---------|
| Покрытие API | 14 эндпоинтов | ✅ 100% |
| Успешность тестов | 100% | ✅ |
| Среднее время ответа | 79-92 мс | ✅ |
| Нагрузка (1000 итераций) | Без ошибок | ✅ |

| Негативные сценарии | 4 теста | ✅ |

### Коллекция: **Reqres**
#### **Get user** (GET запросы):
1. [`user list`](/Practice_on_the_course/04_api_testing_postman/docs/create_user.png) - получение списка пользователей
2. [`single user`](/Practice_on_the_course/04_api_testing_postman/docs/single_user.png) - получение одного пользователя
3. [`min users`](/Practice_on_the_course/04_api_testing_postman/docs/min_user.png) - минимальное количество пользователей
4. [`zero users`](/Practice_on_the_course/04_api_testing_postman/docs/zero_users.png) - пустой список пользователей  
5. [`non-existent user`](/Practice_on_the_course/04_api_testing_postman/docs/non-existent_user.png) - несуществующий пользователь
6. [`pagination`](/Practice_on_the_course/04_api_testing_postman/docs/pagination.png) - пагинация списка

#### **Post user** (POST/PUT/PATCH):
7. [`create user`](/Practice_on_the_course/04_api_testing_postman/docs/create_user.png) - создание пользователя
8. [`register user`](/Practice_on_the_course/04_api_testing_postman/docs/register_user.png) - регистрация пользователя
9. [`update full user`](/Practice_on_the_course/04_api_testing_postman/docs/update_full_user.png) - полное обновление (PUT)
10.[ `update user`](/Practice_on_the_course/04_api_testing_postman/docs/update_user.png) - частичное обновление (PATCH)
11.[ `authorization user`](/Practice_on_the_course/04_api_testing_postman/docs/authorization_user.png) - авторизация
12.[ `negative register user`](/Practice_on_the_course/04_api_testing_postman/docs/negative_register_user.png) - негативная регистрация
13.[ `negative authorization user`](/Practice_on_the_course/04_api_testing_postman/docs/negative_authorization_user.png) - негативная авторизация

#### **Delete** (DELETE запросы):
14. [`delete user`](/Practice_on_the_course/04_api_testing_postman/docs/delete_user.png) - удаление пользователя

## Используемые технологии
- **Postman** - основное тестирование
- **Markdown** - документация
- **Git/GitHub** - версионный контроль