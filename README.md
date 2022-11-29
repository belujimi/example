_______Список участников команды:_______
- Kate Smirnova
- Cherny Oleg
- Mikhail Belugin

_______Имя тимлида (по желанию):_______
- Kate Smirnova

_______Описание выбранной идеи решения:_______
Нарисована модель основной логики  в Visio. ссылка
позднее логика обрастала дополнительными функциями.
такими как:
"накричать на всех"
"выбор языка меню"
"Показать список пользователей"

_______Описание пользовательских типов и функций в проекте:_______
- Пользовательские типы:
- Классы: Chat, Message,User.
- Функций:
- registration_in_the_chat() открывает меню регистрации
- log_ln_to_the_chat() открывает меню входа
- show_chat() показывает чат
- show_all_users_name() показывает всех зарегистрированных пользователей
- add_message() отправить сообщение
- void add_message(char a) отправить сообщение всем
и др.

_______Пояснение, как были распределены задачи в команде (кто какую часть проекта реализовывал):_______
Задачи были распределены по принципу дополнять проект по заранее подготовленному
списку функции по порядку. Зашёл увидел какая не написана - пишешь. Таким образом работа над проектом
не останавливалась по причине отсутствия кого-то в какой-то день.  Нагрузка была распределена равномерно без переработки.

_______Kate Smirnova
- Организация плана работ по проекту
- Установка графика выполнения этапов
- Зарисовка макета(бумага)
- Описание проекта в файлах (подробно)
- Создание классов и заголовочных файлов
- Исправление ошибок кода после дополнений (корректировка)
- Визуализация
- Добавление выбора языка + исправление кодировки ввода вывода
- show_chat() показывает чат
- CAT() вывод ошибок
- NOTCAT() вывод ошибок
- Сеттеры
- Геттеры
- add_message(char a) отправить сообщение всем

_______Cherny Oleg
- Тестирование
- Работа над ошибками имени и логина блоки try catch
- Контроль работы гитхаб
- registration_in_the_chat() открывает меню регистрации
- add_message() отправить сообщение
- start()
- isChatWork()

_______Mikhail Belugin
- Тестирование
- log_ln_to_the_chat()
- Отрисовка о сановной схемы проекта в Visio(по рукописи)
- Тестирование выявление ошибок безопасности
- add_message() отправить сообщение
- showUserMenu()
- menu_message()

_______Контроль версий_______
1.0 Основные файлы

1.1 основная структура программы(описание\макет).

1.1.1 Основные классы и main

1.2 исправлена кодировка
- Умеет заходить в регистрацию.
- Создавать юзера.
- Класть его в вектор юзеров.

1.3 добавлен std::shared_ptr<User> Chat::get_user_by_name
- Добавлен void CAT();
- Испралены блоки try перекидывание exception в меню регестрации.
  
1.4 написаны вход в чат
- вывод чата
- отправка сообщений конкретному пользователю
- Ошибка отправки сообщения всем пользователям!!! или предупредить пользователе что бы писал "всем" или добавить пункт меню для отправки всем.
- Временно присутствует цикл на регистрации нескольких пользователей сразу для удобство отладки.

1.5 исправлены ошибки прошлых версий с двойным вводом пороля
- Убраны лишние комментарии макета.
- Временно убран CAT();(error)
- Тест выявлены проблемы с кодировкой записью в стринг. поток ввода.
- Тест выявлены ошибки рекурсии.
  
1.6 откат до 1.4 (1.5 показательная чистая)
- Исправлены ошибки прошлых версий с двойным вводом пароля.
- Исправлена ошибка взлома.
- Добавлена перегрузка функции void Chat::add_message(char a) для отправки всем.
- Добавлена функция void Chat::shout() наорать на всех с преобразованием текста в капслок + конкатенация строк "!!!!!!!".
- Добавлена функция void Chat::menu_message() меню сообщений.
- Тест выявлены проблемы с кодировкой записью в стринг. поток ввода.???(позднее)
- Тест выявлены возможные ошибки рекурсии.???(позднее)
 
1.7
- Исправлена ошибка кодировки вводимых символов кириллицы.
- Тест выявлены возможные ошибки рекурсии.???(позднее)

1.8
- Исправлена ошибка рекурсии.
- Блоки try catch перенесены в main что закрывает функцию меню.

1.9
- Добавлено меню языка.
- Реализован выбор языка. русский/англисский.
- перевод всей программы на 2 языка.
- Добавленна переменная char language_
- Добавлены фунции void set_language(char language) и char get_language()
- Вся программа локализирована.
- Ошибок нет.
- Ворнинг нет.
  
2.0
- Добавлен краб.
- Коты стали более пушистые.
- работа с визуальной частью.
- Исправления отправки всем замена имени "от я" на "от меня".
- Добавлена функция NOTCAT();

2.1
- работы с цветом.
- Корректировки цвета в англ. меню и русском.
