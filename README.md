# WorldSkillsDemoTrade

Решение одного из вариантов демонстрационного экзамена WorldSkills 2022 года.

## Содержание
* [Описание задания](#описание-задания)
* [Описание предметной области](#описание-предметной-области)
* [Требования и рекомендации](#требования-и-рекомендации)  
    * [Введение](#введение)  
    * [Правила](#правила)  
    * [Название приложения](#название-приложения)
    * [Файловая структура](#файловая-структура)
    * [Структура проекта](#структура-проекта)
    * [Логическая структура](#логическая-структура)
    * [Руководство по стилю](#руководство-по-стилю)
    * [Обратная связь с пользователем](#обратная-связь-с-пользователем)
    * [Обработка ошибок](#обработка-ошибок)
    * [Оформление кода](#оформление-кода)
    * [Комментарии](#комментарии)
    * [Оценка](#оценка)
    * [Предоставление результатов](#предоставление-результатов)
* [Модуль 3: Разработка баз данных, объектов баз данных и импорт](#модуль-3-разработка-баз-данных-объектов-баз-данных-и-импорт)

## Описание задания.
Задачей демонстрационного экзамена является разработка информационной системы для компании.  
Система будет состоять из нескольких модулей, доступ к которым будет определяться типом учетной записи.  
Общее назначение разрабатываемых модулей:
* просмотр списка объектов,
* добавление/удаление/редактирование данных об объектах,
* управление списком возможных объектов.  

## Описание предметной области

ООО «Товары для животных»  - магазин по продаже товаров для животных в Нефтеюганске.
В рамках выполнения задания демонстрационного экзамена необходимо разработать основные модули информационной системы для ООО «Товары для животных»:
*	авторизованный клиент и менеджер может просматривать товары;
*	администратор может добавлять/редактировать/удалять товары.

Кроме того, разрабатываемая Вами информационная система предполагает установку на терминалах при входе в торговые центры города. На терминале клиент (авторизованный и неавторизованный) может просмотреть товары, сформировать заказ и выбрать удобный для него пункт выдачи.


## Требования и рекомендации

### Введение

Для выполнения задач экзаменационного задания вы можете использовать любые инструменты, предоставляемые согласно инфраструктурного листа.
В случае нехватки времени для выполнения всех оставшихся задач вы можете пропускать выполнение некоторых задач в пользу других. Однако ожидается, что вы предоставите максимально завершенную работу в конце каждой сессии, чтобы облегчить оценку вашей работы.

### Правила

Во время проведения экзамена необходимо соблюдать следующие правила:
*	Запрещен доступ в Интернет (кроме разового доступа в течение сессии не более 15 минут);
*	Запрещено использование любых гаджетов (мобильный телефон, планшет, смарт-часы и т.д.);
*	Запрещено использование ваших собственных устройств хранения данных (USB- накопители, жесткие диски и т.д.);
*	Запрещено общение с другими участниками экзамена;
*	Запрещено приносить на экзамен книги, заметки и т.д.;
*	Разрешено использовать личные устройства ввода информации (клавиатура, мышь, трекбол и т.д.), но эти устройства должны быть проводными, непрограммируемыми и должны работать без дополнительной установки драйверов (эти требования предварительно проверяются техническим экспертом);
*	Разрешено использовать личные средства повышения эргономики (коврик для мыши, подставка под запястья и т.д.), а также талисманы (также проходят проверку у технического эксперта);
*	При возникновении любой внештатной ситуации с программным или аппаратным  обеспечением, а также периферийными устройствами необходимо немедленно прервать работу и обратиться к эксперту.

Несоблюдение этих правил может привести к удалению с площадки проведения экзамена.

### Название приложения

Используйте соответствующие названия для ваших приложений и файлов. Так, например, наименование настольного приложения должно обязательно включать название компании- заказчика.

### Файловая структура

Файловая структура проекта должна отражать логику, заложенную в приложение. Например, все формы содержатся в одной директории, пользовательские визуальные компоненты – в другой, классы сущностей – в третьей.

### Структура проекта

Каждая сущность должна быть представлена в программе как минимум одним отдельным классом. Классы должны быть небольшими, понятными и выполнять одну единственную функцию (Single responsibility principle).
Для работы с разными сущностями используйте разные формы, где это уместно.

### Логическая структура
Логика представления (работа с пользовательским вводом/выводом, формы, обработка событий) не должна быть перемешана с бизнес-логикой (ограничения и требования, сформулированные в заданиях), а также не должна быть перемешана с логикой доступа к базе данных (SQL-запросы, запись, получение данных). В идеале это должны быть три независимых модуля.

### Руководство по стилю
Визуальные компоненты должны соответствовать руководству по стилю, предоставленному в качестве ресурсов к заданию в соответствующем файле. Обеспечьте соблюдение требований всех компонентов в следующих областях:
*	цветовая схема,
*	размещение логотипа,
*	использование шрифтов,
*	установка иконки приложения.

**Использование логотипа**

Все экранные формы пользовательского интерфейса должны иметь заголовок с логотипом (в ресурсах). Не искажайте логотип (не изменяйте изображение, его пропорции, цвет).

Также для приложений должна быть установлена иконка.

**Шрифт**

Используйте шрифт Comic Sans MS.

**Цветовая схема**

В	качестве основного фона используется белый цвет; в качестве дополнительного: RGB (118, 227, 131).

Для акцентирования внимания пользователя на целевое действие интерфейса используйте цвет RGB (73, 140,81).

**Макет и технические характеристики**
Все компоненты системы должны иметь единый согласованный внешний вид, соответствующий руководству по стилю, а также следующим требованиям:
*	разметка и дизайн (предпочтение отдается масштабируемой компоновке;
*	должно присутствовать ограничение на минимальный размер окна; 
*	должна присутствовать возможность изменения размеров окна, где это необходимо; 
*	увеличение размеров окна должно увеличивать размер контентной части, например, таблицы с данными из БД);
*	группировка элементов (в логические категории);
*	использование соответствующих элементов управления (например, выпадающих списков для отображения подстановочных значений из базы данных);
*	расположение и выравнивание элементов (метки, поля для ввода и т.д.);
*	последовательный переход фокуса по элементам интерфейса (по нажатию клавиши TAB);
*	общая компоновка логична, понятна и проста в использовании;
*	последовательный пользовательский интерфейс, позволяющий перемещаться между существующими окнами в приложении (в том числе обратно, например, с помощью кнопки «Назад»);
*	соответствующий заголовок на каждом окне приложения (не должно быть значений по умолчанию типа MainWindow, Form1 и тп).

### Обратная связь с пользователем

Уведомляйте пользователя о совершаемых им ошибках или о запрещенных в рамках задания действиях, запрашивайте подтверждение перед удалением, предупреждайте о неотвратимых операциях, информируйте об отсутствии результатов поиска и т.п. Окна сообщений соответствующих типов (например, ошибка, предупреждение, информация) должны отображаться с соответствующим заголовком и пиктограммой. Текст сообщения должен быть полезным и информативным, содержать полную информацию о совершенных ошибках пользователя и порядок действий для их исправления. Также можно использовать визуальные подсказки для пользователя при вводе данных.

### Обработка ошибок

Не позволяйте пользователю вводить некорректные значения в текстовые поля сущностей. Например, в случае несоответствия типа данных или размера поля введенному значению. Оповестите пользователя о совершенной им ошибке.
Обратите внимание на использование абсолютных и относительных путей к изображениям. Приложение должно корректно работать, в том числе и при перемещении папки с исполняемым  файлом.
При возникновении непредвиденной ошибки приложение не должно аварийно завершать работу.

### Оформление кода
Идентификаторы переменных, методов и классов должны отражать суть и/или цель их использования, в том числе и наименования элементов управления (например, не должно быть значений по умолчанию типа Form1, button3).
Идентификаторы должны соответствовать соглашению об именовании (Code Convention) и стилю CamelCase (для C# и Java) и snake_case (для Python).
Допустимо использование не более одной команды в строке.


### Комментарии
Используйте комментарии для пояснения неочевидных фрагментов кода. Запрещено комментирование кода.
Хороший код воспринимается как обычный текст. Не используйте комментарии для пояснения очевидных действий. Комментарии должны присутствовать только в местах, которые требуют дополнительного пояснения.
Используйте тип комментариев, который в дальнейшем позволит сгенерировать XML- документацию, с соответствующими тегами (например, param, return(s), summary и др.)

### Оценка
Каждая задача оценивается путем тестирования реализации требуемого функционала. Так как требования к реализуемой системе очень высоки, возможно, будут использоваться средства для автоматизированного тестирования приложения. В связи с этим, в ходе разработки, может возникнуть необходимость следовать определенным правилам именования и структурирования проекта.

### Предоставление результатов
Все практические результаты должны быть переданы заказчику путем загрузки файлов на предоставленный вам репозиторий системы контроля версий git. Практическими результатами являются:
*	исходный код приложения (в виде коммита текущей версии проекта, но не архивом),
*	исполняемые файлы,
*	прочие графические/текстовые файлы.
Результаты работы каждой сессии должны быть загружены в отдельный репозиторий с названием «Сессия X» (X – номер сессии).
Для оценки работы будет учитываться только содержимое репозитория. При оценке рассматриваются заметки только в электронном виде (readme.md). Рукописные примечания не будут использоваться для оценки.
Проект обязательно должен содержать описание в формате Markdown (см. шаблон в файле README-Template.md или README-Template_rus.md). Заполните также дополнительную информацию о проекте и способе запуска приложения в файле readme.md.
Обратите внимание, что дополнительного времени после окончания сессии на сохранение не предусмотрено, поэтому будьте бдительны и загружайте результаты работ своевременно в рамках сессии.

## Модуль 3: Разработка баз данных, объектов баз данных и импорт


### Импорт исходных данных

Данные, которые нам необходимо импортировать помечены в директории сессии с помощью __\*\_import__

![Директория сессии](/TutorialResources/session_directory.png)

Также, здесь располагается файл со скриптом для СУБД (MS SQL и MySQL):

```
create database [Trade]
go
use [Trade]
go
create table [Role]
(
	RoleID int primary key identity,
	RoleName nvarchar(100) not null
)
go
create table [User]
(
	UserID int primary key identity,
	UserSurname nvarchar(100) not null,
	UserName nvarchar(100) not null,
	UserPatronymic nvarchar(100) not null,
	UserLogin nvarchar(max) not null,
	UserPassword nvarchar(max) not null,
	UserRole int foreign key references [Role](RoleID) not null
)
go
create table [Order]
(
	OrderID int primary key identity,
	OrderStatus nvarchar(max) not null,
	OrderDeliveryDate datetime not null,
	OrderPickupPoint nvarchar(max) not null
)
go
create table Product
(
	ProductArticleNumber nvarchar(100) primary key,
	ProductName nvarchar(max) not null,
	ProductDescription nvarchar(max) not null,
	ProductCategory nvarchar(max) not null,
	ProductPhoto image not null,
	ProductManufacturer nvarchar(max) not null,
	ProductCost decimal(19,4) not null,
	ProductDiscountAmount tinyint null,
	ProductQuantityInStock int not null,
	ProductStatus nvarchar(max) not null,
)
go
create table OrderProduct
(
	OrderID int foreign key references [Order](OrderID) not null,
	ProductArticleNumber nvarchar(100) foreign key references Product(ProductArticleNumber) not null,
	Primary key (OrderID,ProductArticleNumber)
)
```

Проанализировав запрос к БД и предоставленные таблицы, можно заметить несоответствие.  
Построим ER-диаграммы для данных, которые мы хотим импортировать и для предлагаемой структуры БД из запроса.

![ER по скрипту](/TutorialResources/ER_script.png)  
*ER-модель по запросу*

![ER по импортируемым данным](/TutorialResources/ER_importData.png)  
*ER-модель по импортируемым данным*

Несложно заметить, что атрибуты сущностей совпадают не везде, а также сущность Role отсутствует в импортируемых данных.  
Посмотрим, какие именно атрибуты не совпадают:
* в сущности User в импортируемых данных ФИО хранится в одном столбце, в предлагаемом запросе - в разных;
* в импортируемых данных нет связи товаров с заказами;
* в сущности "Заказ" внешний ключ на несуществующий атрибут PointID;
* атрибут ProductCurrentDiscount есть только в сущности "Товар";
* непонятно, что именно означает атрибут ProductStatus. Скорее всего, это отсутствие/наличие на складе, вычислимое значение, зависит от количества товара на складе. Чтобы избавиться от ненужной нам транзитивной зависиммости, уберем этот атрибут.

Информацию о ролях следует уточнить у заказчика, но у нас нет такой возможности, поэтому обусловимся, что 1 - это администратор, 2 - модератор и 3 - пользователь.

Составим новую ER-модель и попробуем нормализовать до третьей формы:

![Новая ER-модель](/TutorialResources/mbGoodER.png)  
*Новая ER-модель*

Информацию о производителе и поставщике оставляем в сущности "Product", так как у нас нет никакой информации, кроме их названия - следовательно, не возникает транзитивной зависимости.  

Теперь подготовим данные к импорту. Начнем с пользователей.

Для начала экспортируем книгу Excel в .csv формат:

![Страница экспорта в Excel](/TutorialResources/ExcelExportPage.png)  
*Страница экспорта в Excel*

Откроем документ с помощью Notepad++. Как мы видим, некоторые строки содержат разделитель в ячейке таблицы:

![Ненужный разделитель](/TutorialResources/DelimiterProblem.png)  
*Ненужный разделитель*

Избавимся от всех подобных неприятностей: откроем csv документ и воспользуемся функционалом Excel для поиска и удаления (Ctrl+H) всех вхождений символа переноса строки. Выделим все ячейки и найдем в них нужный символ. Переносу строки эквивалентно сочетание клавиш Ctrl+J. Вы не увидите сам этот символ, вместо него будет мигающая маленькая точка. Его помещаем в поле "Найти". Поле "Заменить на" оставляем пустым.

![Ненужный разделитель убран](/TutorialResources/DelimiterProblemSolved.png)  
*Ненужный разделитель убран*

Теперь можем приступать к обработке данных. Нам нужно только разделить ФИО на три части и поставить разделитель

Для этого напишем регулярное выражение

![Регулярное выражение для пользователей](/TutorialResources/UserRegularExpression.png)  
*Регулярное выражение для пользователей*

Что же всё это значит? Подробное объяснение всего регулярного выражения и иерархии групп можно найти на https://regex101.com/r/6Udj5Y/2. (*Хороший сайт для проверки своих регулярных выражений*)

![Подготовили пользователей к импорту](/TutorialResources/UsersParsed.png)  
*Подготовили пользователей к импорту*

Удалим последнюю пустую строку и готово - пользователи готовы к импорту.