# План автоматизации

## Перечень автоматизируемых сценариев

### Валидные данные:

* номер карты: 16 цифр
* месяц: 2 цифры в диапазоне от 01 до 12 не ранее текущего месяца
* год: 2 цифры не ранее текущего года
* имя владельца : латинские буквы ,
* cvc/ cvv: 3 цифры

### Позитивные сценарии:

**Оплата по карте**

* Успешное завершение операции при вводе валидных данных и/или действующей карты.
* Ошибка при выполнении операции при вводе валидных данных и/или недействительной карты.

**Кредит по данным карты**

* Успешное завершение операции при вводе валидных данных и/или действующей карты.
* Ошибка при выполнении операции при вводе валидных данных и/или недействительной карты.

### Негативные сценарии:

**Оплата по карте**
* Отправка формы с незаполнеными полями
* Ввод невалидных значений или отправка пустого поля *месяц*
* Ввод невалидных значений или отправка пустого поля *год*
* Ввод невалидных значений или отправка пустого поля *имя владельца*
* Ввод невалидных значений или отправка пустого поля *cvc/cvv*

**Кредит по данным карты**
* Отправка формы с незаполнеными полями
* Ввод невалидных значений или отправка пустого поля *месяц*
* Ввод невалидных значений или отправка пустого поля *год*
* Ввод невалидных значений или отправка пустого поля *имя владельца*
* Ввод невалидных значений или отправка пустого поля *cvc/cvv*

## Перечень используемых инструментов с обоснованием выбора
* *Java* - язык програмирования для написания автотестов
* *IntelliJ IDEA* - интегрированная среда разработки программного обеспечения для многих языков, в частности для Java
* *Junit 5* - фреймворк для модульного тестирования программного обеспечения на языке Java
* *Gradle* -  система для автоматизации сборки приложений
* *Faker* - библиотека с открытым исходным кодом, которая генерирует даннные
* *Selenide* - фреймворк для автоматизированного тестирования
* *Allure* - фрейворк для прросмотра отчетов по тестированию
* *Docker* - Открытая платформа для разработки, доставки и эксплуатации приложений
* *Lombok* - библиотека для сокращения кода в классах и расширения функциональности языка Java
* *Git* - распределенная система управления версиями
* *GitHub* - крупнейший веб-сервис для хостинга IT-проектов и их совместной разработки

## Перечень и описание возможных рисков при автоматизации
* Неоправданная стоимость автоматизации
* Изменение локаторов веб - элементов страницы
* Искажение результатов тестирования в связи с отсутствием доступа к реальным данным пользователей (при использовании Faker)
* Отсутствие документации

## Интервальная оценка с учётом рисков (в часах)
* Подготовка окружения - 10 часов
* Написание и проверка автотестов - 96 часов
* Формирование отчетов - 12 часов

## План сдачи работ
* 26.09.22 - сдача автотестов
* 03.10.22 - устранение ошибок
* 07.10.22 - сдача дипломного проекта