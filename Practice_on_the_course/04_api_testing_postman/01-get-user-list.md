## 📋 Запрос: GET User List

### 🎯 Назначение
Получение информации о всех пользователях

### 🔧 Технические детали
- **Метод:** `GET`
- **Коллекция:** Reqres
- **Окружение:** url, x-api-key
- **Авторизация:** API Key
- **Теги:** `user list`

### 📝 Пример запроса из файла
```http
GET /api/users HTTP/1.1
Host: reqres.in
Authorization: API Key
```
### ✅ Успешный ответ (200 OK)

```json
{
    "page": 1,
    "per_page": 6,
    "total": 12,
    "total_pages": 2,
    "data": [
        {
            "id": 1,
            "email": "george.bluth@reqres.in",
            "first_name": "George",
            "last_name": "Bluth",
            "avatar": "https://reqres.in/img/faces/1-image.jpg"
        },
        {
            "id": 2,
            "email": "janet.weaver@reqres.in",
            "first_name": "Janet",
            "last_name": "Weaver",
            "avatar": "https://reqres.in/img/faces/2-image.jpg"
        },
        {
            "id": 3,
            "email": "emma.wong@reqres.in",
            "first_name": "Emma",
            "last_name": "Wong",
            "avatar": "https://reqres.in/img/faces/3-image.jpg"
        },
        {
            "id": 4,
            "email": "eve.holt@reqres.in",
            "first_name": "Eve",
            "last_name": "Holt",
            "avatar": "https://reqres.in/img/faces/4-image.jpg"
        },
        {
            "id": 5,
            "email": "charles.morris@reqres.in",
            "first_name": "Charles",
            "last_name": "Morris",
            "avatar": "https://reqres.in/img/faces/5-image.jpg"
        },
        {
            "id": 6,
            "email": "tracey.ramos@reqres.in",
            "first_name": "Tracey",
            "last_name": "Ramos",
            "avatar": "https://reqres.in/img/faces/6-image.jpg"
        }
    ]
}
```    

### 🧪 Проверки
```javascript
// Проверка статуса
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

// Проверка заголовков
pm.test("Content-Type is present", function () {
    pm.response.to.have.header("Content-Type");
});

// Проверка времени ответа
pm.test("Response time is less than 200ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(200);
});
```
### 📊 Результаты тестирования
| Метрика |	Значение | Статус |
|-----------|-----------|-----------|
| Статус | код	200 | ✅ PASS |
| Content-Type | Присутствует |	✅ PASS |
| Время ответа | <200 мс | ✅ PASS |
| Общее время |	92 мс |	В пределах нормы |
