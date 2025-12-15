# API Запросы – Коллекция "My Workspace"

---

## 📂 Коллекция: Reqres

### 📌 **GET Запросы**

#### **1. Get user list**
- **Метод:** GET
- **Коллекция:** Reqres
- **Категория:** User list
- **Описание:** Получить список пользователей

---

#### **2. Get single user**
- **Метод:** GET
- **Коллекция:** Reqres
- **Категория:** User list
- **Пример запроса:**
  
{
  "start": "<hackle.nextIdRequest>.ir>",
  "result": "<hackle.nextIdRequest>",
  "first_name": "next1r>",
  "last_name": "next2r>",
  "endset": "https://content.io/img/faculty.faculty.jpg"
}
3. Get min users
Метод: GET

Коллекция: Reqres

Категория: User list

4. Get zero users
Метод: GET

Коллекция: Reqres

Категория: User list

5. Get non-existent user
Метод: GET

Коллекция: Reqres

Категория: User list

Авторизация: API Key

Пример URL: [GET] / Retrieve (12)

6. Get pagination
Метод: GET

Коллекция: Reqres

Категория: User list
📝 POST Запросы
7. Post user / Create user
Метод: POST

Коллекция: Reqres

Категория: Post user

8. Register user
Метод: POST

Коллекция: Reqres

Категория: Post user

Пример тела запроса:

json
{
  "email": "eve.holt@reqres.in",
  "password": "pistol"
}
Пример ответа (201 Created):

json
{
  "user": "localhost",
  "job": "Tasker",
  "test:tasker": "",
  "test:start": "2005-12-04T17:10:44.4027"
}
9. Update full user
Метод: PUT

Коллекция: Reqres

Категория: Post user

10. Update user
Метод: PATCH

Коллекция: Reqres

Категория: Post user

11. Authorization user
Метод: POST

Коллекция: Reqres

Категория: Post user

Пример ответа:

json
{
  "GET ": "token": "YourList<String>Error"
}
12. Negative register user
Метод: POST

Коллекция: Reqres

Категория: Post user

Параметры:

form-data

x-xview-form-reincredited

Пример тела:

json
{
  "Access": "Missing password"
}
Ответ: 400 Bad Request (1.5 KB)

13. Negative authorization user
Метод: POST

Коллекция: Reqres

Категория: Post user

🗑️ DELETE Запросы
14. Delete user
Метод: DELETE

Коллекция: Reqres

Категория: Delete

Параметры:

form-data

e-mailed-form-releaseded

Пример:

text
Name: "localhost",
Type: "localhost"
Ответ: 204 No Content (1.2.7 KB)

🧪 Результаты тестирования
Запуск 1 (08:24:40 PM)
Метод	Запрос	Результат	Проверки
GET	user list	✅ PASS	Status 200, Content-Type present
GET	single user	✅ PASS	Status 200, Content-Type present
GET	min users	✅ PASS	Status 200, Content-Type present
GET	zero users	✅ PASS	Status 200, Content-Type present
GET	non-existent user	✅ PASS	Status 200, Content-Type present
GET	pagination	✅ PASS	Status 200, Content-Type present
POST	create user	✅ PASS	Status 200, Content-Type present
POST	register user	✅ PASS	Status 200, Content-Type present
PUT	update full user	✅ PASS	Status 200, Content-Type present
PATCH	update user	✅ PASS	Status 200, Content-Type present
POST	authorization user	✅ PASS	Status 200, Content-Type present
POST	negative register user	✅ PASS	Status 200, Content-Type present
POST	negative authorization user	✅ PASS	Status 200, Content-Type present
DELETE	delete user	✅ PASS	Status 200, Content-Type present
Общие проверки для всех запросов:

✅ Status code is 200

✅ Content-Type is present

❌ FAIL: Response time is less than 200ms (не пройдено)

Запуск 2 (08:35:44 PM, нагрузочное тестирование)
Итераций: 1000

Длительность: 3m 13s

Всего тестов: 3000

Среднее время ответа: 79 ms

📊 Сводка по типам запросов
Тип	Количество	Статус
GET	6	✅ Все протестированы
POST	6	✅ Все протестированы
PUT	1	✅ Протестирован
PATCH	1	✅ Протестирован
DELETE	1	✅ Протестирован
Всего	15	✅ 100% покрытие
🔗 Другие коллекции в рабочем пространстве
Search collections:
Dadata

HeadHunter

Lers

Placeholder

Postman

Reqres (активная)

User management categories:
User list (6 запросов)

Post user (7 запросов)

Delete (1 запрос)


