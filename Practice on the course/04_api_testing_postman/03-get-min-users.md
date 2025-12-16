# 📋 Запрос: GET Min Users

## 🎯 Назначение
Получение минимального количества пользователей

## 🔧 Технические детали
- **Метод:** `GET`
- **Коллекция:** Reqres 

## 📋 🎯 Цель теста
Проверка корректности работы API при:
- Минимальном количестве возвращаемых данных
- Корректной работе пагинации
- Сохранении структуры ответа

## 🧪 Проверки (no testing)
```javascript
pm.test("Returns users when min count requested", function () {
    const response = pm.response.json();
    pm.expect(response.data).to.be.an('array');
    pm.expect(response.data.length).to.be.above(0);
});

pm.test("Pagination works with min users", function () {
    const response = pm.response.json();
    pm.expect(response).to.have.property('total');
    pm.expect(response).to.have.property('per_page');
});
```
## Успешный ответ (200 OK)
```json
{
    "data": {
        "id": 1,
        "email": "george.bluth@reqres.in",
        "first_name": "George",
        "last_name": "Bluth",
        "avatar": "https://reqres.in/img/faces/1-image.jpg"
    },
    "support": {
        "url": "https://contentcaddy.io?utm_source=reqres&utm_medium=json&utm_campaign=referral",
        "text": "Tired of writing endless social media content? Let Content Caddy generate it for you."
    },
    "_meta": {
        "powered_by": "🚀 ReqRes - Deploy backends in 30 seconds",
        "upgrade_url": "https://app.reqres.in/upgrade",
        "docs_url": "https://reqres.in",
        "template_gallery": "https://app.reqres.in/templates",
        "message": "This API is powered by ReqRes. Deploy your own backend in 30 seconds!",
        "features": [
            "30 Second Backend Templates",
            "Custom API Endpoints",
            "Data Persistence",
            "Real-time Analytics"
        ],
        "upgrade_cta": "Upgrade to Pro for unlimited requests, custom endpoints, and data persistence"
    }
}
```
