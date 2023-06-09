В рамках дисциплины "Инфокомуникационные системы и сети" в университете, была реализована база данных склада.
![image](https://github.com/daktanaev/1C/assets/105858525/7deed203-1842-479d-9502-10f54f209e71)

В процессе обучения изучил следующие пункты:

Задание 1. Доработка конфигурации "Склад"
1) создал журнал документов;
2) создал подсистемы;
3) в отчете дополнительно сделал отбор по цвету и стране с необязательностью выбора.
![image](https://github.com/daktanaev/1C/assets/105858525/8b191934-f96e-4c98-9161-7cd1b8c732a3)


Задание 2. Доработка конфигурации "Склад" (обработка 1)
1) В команду "ЗаменаЦвета" внес изменения в программный код, позволяющие избавиться от перебора в цикле всех элементов справочника Товары. Таким образом, необходимо в метод Выбрать (ВыборкаТоваров = Справочники.Товары.Выбрать();) добавил аргумент Отбор, по которому в нашу выборку будут попадать только товары красного цвета.
2) В замену страны добавил возможность выбора желаемой категории товаров, для которых нужно заменить страну. При этом нельзя давать возможность указать не папку, а элемент (товар).

Задание 3. Доработка конфигурации "Склад" (обработка 1)
1) Корректировка процедуры СоздатьГруппуНаСервере(). При создании новой группы реализовать проверку на существование группы с таким же именем. Если такая уже существует, выдавать предупреждение и не создавать.
2) Модифицировать процедуру УдалитьТоварНаСервере() таким образом, чтобы выводилась информация, в каких документах есть ссылки на удаляемый товар.
3) В код процедуры ВыгрузитьТекстНаСервере() добавить выгрузку цвета и страны.

Задание 4. Доработка конфигурации "Склад" (обработка 1 - загрузка из текст. файла)
1) Дополнить процедуру "ЗагрузитьТекстНаСервере" импортом из файла цвета и страны.
2) Не загружать в 1С одинаковые товары.

Задание 5. Доработка конфигурации "Склад" (обработка 1 - документ - загрузка/выгрузка данных)
1) Реализовать выгрузку данных из документа в текстовый файл.
2) Реализовать загрузку данных из текстового файла в новый документ.

Задание 6. Доработка конфигурации "Склад" (обработка 1 - документ - Документ1НаСервере)
1) Задать пользователю вопрос по непроведенному документу, хочет ли он его провести.
2) Исправить ситуацию, когда документ проводится в любом случае.

Задание 7. Доработка конфигурации "Склад" (первый запуск)
1) Необходимо изменить логику таким образом, чтобы форма первого запуска не запускалась для администратора (вне зависимости от значения константы ПервыйЗапускОсуществлен).
2) Необходимо добавить для складов реквизит инвентаризация (тип Дата) и на форме первого запуска показывать информацию о том, у каких складов сегодня инвентаризация.

Задание 8. Доработка конфигурации "Склад" (ПереносИзОднойГруппыВДругуюНаСервере)
Необходимо изменить процедуру ПереносИзОднойГруппыВДругуюНаСервере() таким образом, чтобы в выборку попадали только товары со страной Россия (через изменение в запросе).
![image](https://github.com/daktanaev/1C/assets/105858525/e67de388-fdc8-412a-8f60-a222b921a176)
