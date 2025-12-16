## 📋 Запрос: GET Single User

### 🎯 Назначение
Получение информации о конкретном пользователе

### 🔧 Технические детали
- **Метод:** `GET`
- **Коллекция:** Reqres → Get user
- **Окружение:** url, x-api-key
- **Авторизация:** API Key
- **Теги:** `single user`

### 📝 Пример запроса из файла
```http
GET /api/users/5 HTTP/1.1
Host: reqres.in
Authorization: API Key
```
### Успешный ответ (200 OK)
```json
{
    "data": {
        "id": 5,
        "email": "charles.morris@reqres.in",
        "first_name": "Charles",
        "last_name": "Morris",
        "avatar": "https://reqres.in/img/faces/5-image.jpg"
    },
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
