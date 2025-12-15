# Отчёт о тестировании API (Postman) — Работа 5

## 📌 Общая информация
- **Автор:** Черкасов Игорь Алексеевич  
- **Дата тестирования:** 04.12.2025  
- **Инструмент:** Postman  
- **Тестируемый API:** Reqres.in (имитация REST API)  
- **Цель:** Проверка функциональности, производительности и обработки ошибок

---

## 🧪 Тестовые коллекции и запросы

### 📁 Коллекция: Reqres

#### **GET запросы:**

1. **Get user list**  
GET /api/users

- Тестовые случаи:
  - single user
  - min users  
  - zero users
  - non-existent user
  - pagination

2. **Get single user** 
GET /api/users/{id}

- Пример: `/api/users/2`

3. **Get non-existent user**
GET /api/users/999

- Проверка на 404

#### **POST запросы:**

4. **Create user**
POST /api/users

text

{
  "name": "morpheus",
  "job": "leader"
}
5. **Register user**
POST /api/register
{
  "email": "eve.holt@reqres.in",
  "password": "pistol"
}
6. **Register user (negative)**
POST /api/register
{
  "email": "sydney@fife"
}
Ожидается ошибка 400
