# Технiчний опис проєкту

Вашiй командi пропонується розробити “Персонального помічника” з інтерфейсом командного рядка.

Основний функцiонал

“Персональний помічник” повинен вміти:

Зберігати контакти з іменами, адресами, номерами телефонів, email та днями народження до книги контактів.
Виводити список контактів, у яких день народження через задану кількість днів від поточної дати.
Перевіряти правильність введеного номера телефону та email під час створення або редагування запису та повідомляти користувача у разі некоректного введення.
Здійснювати пошук контактів серед контактів книги.
Редагувати та видаляти записи з книги контактів.
Зберігати нотатки з текстовою інформацією.
Проводити пошук за нотатками.
Редагувати та видаляти нотатки.

Основні вимоги до Персонального помічника:

1. Зберігання та управління контактами:

Додавання нових контактів із іменами, адресами, номерами телефонів, електронною поштою та днями народження.
Пошук контактів за різними критеріями (наприклад, за іменем).
Редагування та видалення контактів.
Виведення списку контактів, у яких день народження через задану кількість днів від поточної дати.
Валідація номера телефону та електронної пошти під час додавання або редагування контакту.

2. Зберігання та управління нотатками:

Можливість додавання текстових нотаток.
Пошук, редагування та видалення нотаток.

3. Зберігання даних:

Всі дані (контакти, нотатки) повинні зберігатися на жорсткому диску у папці користувача.
Помічник може бути перезапущений без втрати даних.

Додатковий функцiонал

Ви також можете розширити/змінити функціонал проєкту на свій розсуд. Ми пропонуємо додаткове ускладнене завдання для тих, хто реалізує основний функціонал.

Хоча додаткове завдання не є обов'язковим, його коректна реалізація може принести вашій команді додаткові 15 балів.

Ну і звісно ж, окрім оцінки - це для вас чудовий шанс спробувати реалізувати більш просунутий функціонал і отримати щодо нього зворотний зв'язок і поради щодо поліпшення. 💪

Тому рекомендуємо не залишати без уваги те, що допоможе вам удосконалювати свої навички.

“Персональний помічник” повинен додатково вміти:

Додавати в нотатки "теги", ключові слова, що описують тему та предмет запису;
Здійснювати пошук та сортування нотаток за ключовими словами (тегами);
Бот повинен аналізувати введений текст і намагатися вгадати, що хоче від нього користувач і запропонувати найближчу команду для виконання

# Додаткові вимоги до Персонального помічника:

1. Зберігання та управління нотатками:

Додавання "тегів" до нотаток.
Пошук та сортування нотаток за "тегами".


2. Інтелектуальний аналіз:

Помічник повинен вгадувати, що хоче від нього користувач, на основі введеного тексту та пропонувати найближчу команду для виконання.

Удачі вам!

Ми з нетерпінням чекаємо побачити, як ви зробите цей проєкт своїм незабутнім успіхом! 🚀

# Критерії прийому роботи
Проєкт розташований у загальнодоступному репозиторії на GitHub (можна використати альтернативу таку як GitLab або BitBucket).
Наявність коментарів та документації до коду. Присутня докладна інструкція щодо встановлення та використання застосунку описана в файлі Readme.md.
Проєкт можна встановити як Python-пакет та викликати з будь-якого місця системи.
Коректність реалізації всіх вимог. Всі вимоги, описані вище, хоча б частково реалізовано.
Інтерфейс користувача реалізовано в вигляді командного рядка.
Інтерфейс користувача базується на текстових повідомленнях та командах, які користувач вводить з клавіатури.
Зручність та логічність інтерфейсу командного рядка.
Програма взаємодіє з користувачем в циклі, пропонуючи вибрати команду та обробляючи її, поки користувач не введе команду для виходу.
Дані коректно зберігаються на жорсткому диску і не втрачаються після перезапуску помічника.
Відсутність помилок у коді при виконані застосунку.
Програма повинна коректно обробляти некоректне введення даних користувача без закриття програми.
Ефективність використання ООП, спадкування та композиції.
Правильна реалізація валідації для кожного поля.
Код повинен бути чистим, структурованим та дотримуватися стандартів PEP 8.


------------------------------------------------------------------
# Command Functions:
General Interaction

hello
exit
close

Contact Management
Adding Contacts
add <name> <phone> [address] [email] [birthday]:

add John 1234567890 1234ElmSt john@example.com 05.12.1985

add Jeine 1515151515 1987ArreySt jaine@example.com 15.02.1984

add Simon 6564987854 2568MorsSt simon@example.com 08.09.1991

Changing Phone Numbers
change John 0987654321

Viewing Phone Numbers
phone John

Showing All Contacts
all

Birthday Management

Show or change Birthday
birthday John 12.05.1990

Listing Upcoming Birthdays
birthdays 5

Deleting Contacts
delete John

Note Management
Adding Notes

add_note Meeting "Discuss project goals"
add_note Meeting "Meeting with John"

Finding Notes
find_note Meeting 

show_notes

Editing Notes
edit_note Meeting "Discuss project objectives"

Adding Tags to Notes
add_tag Meeting project

Searching Notes by Tags
search_by_tag project

Deleting Notes
delete_note Meeting


exit
close