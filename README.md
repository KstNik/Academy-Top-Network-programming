# Academy-Top-Network-programming

#### Курсовая работа

## CourseWork

Создать файловый менеджер с сетевой синхронизацией – приложение, которое позволяет пользователям управлять своими файлами и папками на локальном компьютере, а также синхронизировать их с удалённым сервером или облачным хранилищем. Такие приложения часто используются для обеспечения резервного копирования данных, доступа к файлам с различных устройств и общего использования файлов между несколькими пользователями.    
Основные функции файлового менеджера с сетевой синхронизацией:    
▪ синхронизация локальных файлов с удалённым сервером или облачным хранилищем;    
▪ резервное копирование файлов на удалённый сервер для защиты данных;    
▪ восстановление файлов из резервных копий в случае утраты данных;    
▪ обмен файлами между пользователями через общий доступ.    
*Примечание:
1. Приложение некорректно передаёт сложные файлы, например такие как Microsoft Office.
2. Имена файлов не должны содержать пробелы.*

#### Решения домашних заданий

## Homework 01

### Тема: "Сокеты"

Задание 1. Переведите первое практическое задание из консольного интерфейса в оконный интерфейс.

Задание 2. Переведите второе практическое задание из консольного интерфейса в оконный интерфейс.

Задание 3. Создайте набор оконных приложений. Первое приложение – сервер, второе приложение клиент. Пользователь вводит в элементы управления информацию об IP-адресе для подсоединения и номере порта. После нажатия на кнопку Подсоединиться клиент подключается к серверу. Если соединение успешно, клиент и сервер могут обмениваться сообщениями до тех пор, пока один из них не попрощается, послав строку Bye. После отсылки этой строки, соединение должно быть закончено. Реализуйте несколько режимов отсылки сообщений:    
▪ Человек (в клиентском приложении человек вводит строку) – человек (в серверном приложении человек вводит строку);    
▪ Человек (клиент) – компьютер (сервер);    
▪ Компьютер (клиент) – человек (сервер);    
▪ Компьютер (клиент) – компьютер (сервер).    
Для реализации ответов компьютера используйте набор заготовленных фраз, выбранных случайным образом.    
Проектируйте архитектуру вашего приложения таким образом, чтобы сетевой блок кода не был завязан на UI. Например, чтобы его было просто перенести из оконного в консольное приложение.

## Homework 02

### Тема: "TCP и UDP сокеты"

Задание 1. Создайте серверное приложение с помощью, которого можно узнавать кулинарные рецепты. Типичный пример работы    
▪ клиентское приложение подключается к серверу;    
▪ клиентское приложение посылает запрос с указанием списка продуктов;    
▪ сервер возвращает рецепты, содержащие указанные продукты;    
▪ клиент может послать новый запрос или отключиться.    
Одновременно к серверу может быть подключено большое количество клиентов. Используйте UDP сокеты для решения этой задачи.

Задание 2. Добавьте к первому заданию ограничение по количеству запросов для конкретного клиента за определённый промежуток времени. Например, клиент не может послать больше, чем 10 запросов за час.

Задание 3. Добавьте к первому заданию ограничение по количеству, одновременно подключённых клиентов. Если какой-то клиент не активен в течение 10 минут он должен быть отключён.

Задание 4. Добавьте оконный интерфейс для управления сервером. Также добавьте оконный интерфейс для управления клиентом.

Задание 5. Добавьте механизм логгирования в сервер. Этот механизм должны сохранять информацию о клиентах, их запросах, времени соединения и т.д.

Задание 6. Добавьте в ответ сервера картинку финального блюда. Например, если сервер возвращает рецепт салата Цезарь, нужно послать клиенту сам рецепт, а также изображение уже готового салата Цезарь.

## Homework 03

### Тема: "Сокеты в С++"

Задание. Разработать и реализовать простое клиент-серверное приложение, в котором клиент отправляет трёхзначное десятичное число на сервер, а сервер возвращает ответ в виде фразы, объясняющей состояние HTTP.    
Например, клиент отправляет числа 200, 401 и 400, а сервер возвращает ответы «Запрос успешно обработан», «Ошибка аутентификации», «Неверный формат запроса».

## Homework 04

### Тема: "Unicast, Multicast, Broadcast"

Задание 1. Создайте оконное приложение «Чат». Для входа в чат пользователи указывают логин. Каждый пользователь видит все сообщения чата. Сообщения в чате могут быть только текстовыми.

Задание 2. Добавьте к первому заданию возможность регистрации по логину и паролю.

Задание 3. Добавьте возможность общения один на один. В этом режиме два пользователя посылают сообщения друг другу и никто, кроме них, их не видит.

Задание 4. Добавьте возможность создания комнат для общения. В комнате может находиться от 1 до N-пользователей.

#### Работа на уроках

## Workinclass 01

### Тема: "Сокеты"

Задание 1. Разработайте два консольных приложения, использующих сокеты. Одно приложение – сервер, второе – клиент. Клиентское приложение посылает приветствие серверу. Сервер отвечает. И клиент, и сервер отображают полученное сообщение. Пример вывода:    
Сервер:    
В 10:25 от [IP-адрес] получена строка: Привет, сервер!    
Клиент:    
В 10:26 от [IP-адрес] получена строка: Привет, клиент!    
Используйте механизм синхронных сокетов.

Задание 2. Разработайте набор консольных приложений. Первое приложение: серверное приложение, которое на запросы клиента возвращает текущее время или дату на сервере. Второе приложение: клиентское приложение, запрашивающее дату или время. Пользователь с клавиатуры определяет, что нужно запросить. После отсылки даты или времени сервер разрывает соединение. Клиентское приложение отображает полученные данные.    
Используйте механизм синхронных сокетов

Задание 3. Измените первое задание, заменив синхронные сокеты на асинхронные.

Задание 4. Измените второе задание, заменив синхронные сокеты на асинхронные.

## Workinclass 02

### Тема: "TCP и UDP сокеты"

Задание 1. Создайте серверное приложение «Генератор цитат» и клиента для получения данных. При запросе клиента, серверное приложение должно вернуть случайную цитату. Процесс должен продолжаться до тех пор, пока клиент не захочет отсоединиться. К одному серверу в один момент времени может быть подключено большое количество клиентов. Сервер ведёт лог соединений:    
▪ Кто подключился;    
▪ Когда подключился;    
▪ Набор цитат;    
▪ Время отключения.  
Клиентское приложение отображает пользователю полученные цитаты. Архитектура вашего приложения должна быть построена без привязки сетевой части к UI. Это означает, что сетевой блок кода может быть легко перемещён в любой вид приложения: консольное, оконное.

Задание 2. Добавьте к первому заданию ограничение по максимальному количеству цитат для пользователя. Когда количество достигнуто, сервер сообщает клиенту об этом и рвёт соединение.

Задание 3. Добавьте к первому заданию ограничение на максимальное количество подключённых клиентов. Когда количество достигнуто, при попытке нового подключения сервер сообщает клиенту, что он сейчас находится под максимальной нагрузкой и необходимо попробовать подключиться через какое-то время.

Задание 4. Добавьте к первому заданию пароль и имя пользователя для подключения. Если пароль и имя пользователя неизвестны, клиент подключиться не может.

## Workinclass 03

### Тема: "Unicast, Multicast, Broadcast"

Задание 1. Создайте систему рассылки информационных сообщений внутри компании. Система состоит из двух приложений. Клиентское приложение используется для получения сообщений. Серверное приложение позволяет ввести и разослать сообщение. Клиент и сервер должны быть реализованы в виде консольных приложений. Проектируйте сетевую архитектуру системы таким образом, чтобы она не зависела от вида приложения и была легко переносима в другой вид приложения.

Задание 2. Добавьте к первому заданию оконный интерфейс клиента.

Задание 3. Добавьте к первому заданию оконный интерфейс для сервера.

Задание 4. Добавьте к первому заданию возможность подписки на конкретный вид сообщений. Клиент определяет, какой тип сообщений он готов получать. Сервер рассылает клиентам только те сообщения, на которые они подписаны.

## Workinclass 04

### Тема: "HTTP, SMTP, FTP"

Задание 1. Создайте оконное приложение, которое по нажатию на кнопку загружает текст Гамлета Шекспира из https://www.gutenberg.org/.    
Когда текст загружен, его нужно отобразить в приложении.    
https://www.gutenberg.org/ – Проект Гуттенберга. Библиотека, в которой более 60000 бесплатных электронных книг.

Задание 2. Создайте оконное приложение, которое позволит, отобразить 100 самых популярных книг из библиотеки Гуттенберга. По нажатию на название книги нужно отобразить текст этой книги.

Задание 3. Создайте приложение для поиска информации в библиотеке Гуттенберга. Пользователь вводит текст для поиска (например, название книги), результаты поиска отображаются в интерфейсе приложения.
