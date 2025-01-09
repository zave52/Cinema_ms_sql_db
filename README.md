# Cinema Database Project

## Проектування та Розробка Бази Даних «Кінотеатр»

Цей репозиторій містить повний набір SQL-скриптів, необхідних для створення, налаштування та управління базою даних для курсової роботи на тему **«Проектування та розробка бази даних «Кінотеатр»»**. База даних призначена для ефективного управління інформацією про кінотеатри, фільми, сеанси, квитки, клієнтів та інші пов'язані сутності.

## Зміст Репозиторію

Репозиторій структурований наступним чином:

- **`tables.txt`**  
  Скрипти для створення основних таблиць бази даних, включаючи визначення полів, типів даних, ключів та зв'язків між таблицями.

- **`history_table.txt`**  
  Скрипти для налаштування системного версіонування таблиць, що дозволяє відстежувати історію змін даних у таблицях `Movies` та `Promotions`.

- **`select.txt`**  
  Приклади SQL-запитів для отримання даних з різних таблиць бази даних, включаючи складні запити з використанням об'єднань та фільтрації.

- **`set_procedures.txt`**  
  Скрипти для створення збережених процедур (`stored procedures`), які забезпечують додавання та оновлення записів у різних таблицях бази даних.

- **`insert.txt`**  
  Скрипти для внесення початкових даних до таблиць бази даних, що включають інформацію про жанри, режисерів, фільми, зали, місця, клієнтів, ролі працівників, товари в магазині, сеанси, відгуки клієнтів, акції та програми лояльності.

- **`stored_procedures.txt`**  
  Скрипти для створення складних збережених процедур, які виконують операції покупки квитків, продажу товарів, планування сеансів та додавання відгуків клієнтів.

- **`views.txt`**  
  Скрипти для створення представлень (`views`), які спрощують доступ до часто використовуваних даних, таких як вільні місця, фільми з найбільшою кількістю проданих квитків, активні пропозиції, доступні фільми, дохід за кожен сеанс та відгуки клієнтів.

- **`get_procedures.txt`**  
  Скрипти для створення збережених процедур, що дозволяють пагінацію, фільтрацію та сортування даних у таблицях, таких як ролі працівників, жанри та категорії продуктів.

## Вимоги

- **Системне ПЗ:** Microsoft SQL Server (версія 2016 або новіша рекомендується).
- **Інструменти:** SQL Server Management Studio (SSMS) або будь-який інший інструмент для виконання SQL-скриптів.
- **Права Доступу:** Необхідні права для створення та модифікації таблиць, процедур, представлень та вставки даних.

## Інструкції з Встановлення

1. **Клонування Репозиторію**

   ```bash
   git clone https://github.com/your-username/cinema-database-project.git
   cd cinema-database-project
   ```

2. **Налаштування Бази Даних**

   - Відкрийте SQL Server Management Studio (SSMS).
   - Створіть нову базу даних, наприклад, `CinemaDB`.

     ```sql
     CREATE DATABASE CinemaDB;
     GO
     ```

3. **Виконання Скриптів Створення Таблиць**

   - Відкрийте файл `tables.txt` та виконайте його в контексті бази даних `CinemaDB`.

4. **Налаштування Історичних Таблиць**

   - Відкрийте файл `history_table.txt` та виконайте його для налаштування системного версіонування таблиць `Movies` та `Promotions`.

5. **Вставка Початкових Даних**

   - Відкрийте файл `insert.txt` та виконайте його для заповнення таблиць початковими даними.

6. **Створення Збережених Процедур та Представлень**

   - Відкрийте файли `set_procedures.txt`, `stored_procedures.txt`, `views.txt`, та `get_procedures.txt` та виконайте їх для створення необхідних процедур та представлень.

7. **Тестування Функціональності**

   - Виконайте приклади викликів процедур з відповідних файлів для перевірки функціональності бази даних.

## Структура Репозиторію

├── tables.txt 

├── history_table.txt

├── select.txt

├── set_procedures.txt

├── insert.txt

├── stored_procedures.txt

├── views.txt

└── get_procedures.txt

## Використання

Після налаштування бази даних ви можете використовувати збережені процедури для управління даними. Наприклад:

- **Додавання/Оновлення Працівників:** `sp_SetEmployee`
- **Покупка Квитка:** `PurchaseTicket`
- **Продаж Товарів:** `SellStoreProduct`
- **Планування Сеансу:** `ScheduleSession`
- **Додавання Відгуку Клієнта:** `AddCustomerFeedback`
- **Отримання Ролей Працівників:** `GetEmployeeRoles`
- **Отримання Жанрів:** `GetGenres`
- **Отримання Категорій Продуктів:** `GetProductCategories`

## Ліцензія

Цей проект ліцензований за ліцензією [MIT](LICENSE).

## Контакти

Для будь-яких запитань або пропозицій, будь ласка, звертайтесь до [your.email@example.com](mailto:your.email@example.com).

