-----------------------------------------------------------------------------------------------------------------

# Графічний додаток для тестування:

Програма створена для проходження тестів. 
За замовчуванням є 2 тести на знання `C#` та `Python`.
Виконання дозволяє добавляти тести, просто добавляючи `JSON-файли` в папку `json`.
В кінці буде виведене отримане *ім'я користувача*, *час проходження* та *оцінка*.
Також є можливість переглянути правильність відповідей.

-----------------------------------------------------------------------------------------------------------------

# Використання:

- Головна сторінка вибору тестів знаходиться в файлі *main.py*.
- З переліку завантажених тестів необхідно обрати потрібний.
- Результати будуть записані в `result.csv`. 
- За надобності його можна видалити і він створиться знову.
- Результати не будуть збережені за відсутності імені (проти анонімності).
- Переглянути правильність відповідей можна після тесту, нажавши на `результат`.
- Результат зберігається та стає доступним після проходження тесту.

-----------------------------------------------------------------------------------------------------------------

# Реалізовані ідеї:

Програма дає змогу додавати тести в форматі `JSON`.
Ім'я буде взято з назви файлу.
Реалізовано це за допомогою вбудованого модуля `glob()`.
Код перебирає імена `.json` файлів та формує список тестів.

Файл `test.py` універсальний для кожного тесту.
Реалізовано це за допомогою форматування.
Тобто ім'я файлу стає змінною, що передається в функцію.
Сильна зав'язка на іменах, але зручно і компактно.

-----------------------------------------------------------------------------------------------------------------