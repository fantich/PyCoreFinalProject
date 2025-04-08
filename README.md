# PyCoreFinalProject
PyCore Final Team Project 

Персональний Помічник

Ласкаво просимо до проєкту "Персональний Помічник" — консольної програми, яка допомагає зберігати та управляти контактами й нотатками. Цей додаток створено для зручного ведення адресної книги та організації текстових записів.

Мета проєкту
Створити систему для:

  *  Зберігання контактів (імена, адреси, номери телефонів, email, дні народження).
  *  Управління нотатками (додавання, пошук, редагування, видалення).
  *  Збереження даних на диску з можливістю перезапуску без втрати інформації.

Встановлення
Вимоги

  *  Python 3.8 або новіша версія.
  *  Операційна система: Windows, macOS, Linux.

Інструкція

  1.  Клонування репозиторію:
 
    git clone https://github.com/SergiyGoIT/PyCoreFinalProject.git
    cd PyCoreFinalProject

 2. Встановлення залежностей: Наразі проєкт не потребує зовнішніх бібліотек, але якщо вони будуть додані, виконайте:

    pip install -r requirements.txt

 3. Запуск програми:

    python src/main.py

Використання

Після запуску програми з’явиться консольне меню з доступними командами. Основні функції:

  *  Додавання контакту: Введіть ім’я, адресу, телефон, email і день народження.
  *  Пошук контактів: Знайдіть контакт за іменем.
  *  Перегляд днів народження: Отримайте список контактів, у яких день народження через задану кількість днів.
  *  Редагування/видалення контактів: Змінюйте або видаляйте записи.
  *  Робота з нотатками: Додавайте, шукайте, редагуйте або видаляйте текстові нотатки.

Приклад команди:


Введіть команду: додати контакт
Ім’я: Іван
Телефон: +380991234567
...
Контакт успішно додано!


Основні функції

  1.  Управління контактами:
     *   Додавання контактів із валідацією телефону (+380xxxxxxxxx) та email (наявність @ і домену).
     *  Пошук, редагування та видалення контактів.
     *   Виведення списку контактів із найближчими днями народження.
  2.  Управління нотатками:
     *   Додавання, пошук, редагування та видалення нотаток.
  3.  Збереження даних:
     *   Контакти та нотатки зберігаються у файлах (наприклад, contacts.json, notes.json) у папці data.

Структура проєкту


PersonalAssistant/
│
├── src/              # Основний код програми
│   ├── main.py       # Точка входу в програму
│   ├── contacts.py   # Логіка роботи з контактами
│   ├── notes.py      # Логіка роботи з нотатками
│   └── storage.py    # Збереження та завантаження даних
│
├── data/             # Папка для зберігання даних
│   ├── contacts.json # Файл із контактами
│   └── notes.json    # Файл із нотатками
│
├── README.md         # Документація
└── .gitignore        # Файл для ігнорування непотрібних файлів

Додаткові можливості (опціонально)

  *  Теги для нотаток: Додавайте ключові слова до нотаток для зручного пошуку.
  *  Пошук і сортування за тегами: Шукайте та впорядковуйте нотатки за тегами.
  *  Інтелектуальний аналіз: Програма намагається вгадати команду на основі введеного тексту (наприклад, "додай замітку" → пропозиція створити нотатку).

Відомі проблеми

  *  Якщо файли даних (contacts.json, notes.json) пошкоджені, програма може завершити роботу з помилкою. Рекомендується додати резервне копіювання.
  *  Валідація телефону підтримує лише український формат (+380xxxxxxxxx).

Розробники

    [Ім’я тім ліда] — координатор проєкту.
    [Ім’я розробника 1] — розробка логіки контактів.
    [Ім’я розробника 2] — розробка логіки нотаток.
    [Ім’я розробника 3] — збереження даних і тестування.

Як внести вклад

  1.  Створіть форк репозиторію.
  2.  Додайте зміни у новій гілці (git checkout -b feature/назва-зміни).
  3.  Створіть pull request із описом змін.