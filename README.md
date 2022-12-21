**CheckRunner** консольное приложение, реализующее функционал формирования чека в магазине.

Для формирования чеков приложению необходимо передать ряд параметров:

- Перечень товаров;

- Номер дисконтной карты (при наличии);

- Путь вывода чека (консоль/файл);

Передать параметры возможно двумя способами:

**Способ 1.** Передача параметров из командной строки при запуске приложения;

**Способ 2.** Передача параметров и файла.

Теперь подробнее.

**Способ 1.** Передача параметров из командной строки при запуске приложения;

Параметры указываются в командной строке при запуске приложения и разделяются пробелами.

> Пример:
> 
> _java_ _CheckRunner  <параметр1> <параметр2> <параметр3>_ и т.д.

Перечень товаров возможно вводить в формате _<__ID_ _товара>-<Количество>._

> Пример:
> 
> _java CheckRunner  3-1 2-5 5-1_

Номер дисконтной карты возможно вводить в формате _< card >-< Номер карты >_

> Пример:
> 
> _java CheckRunner  3-1 2-5 5-1 Card-123_

Путь вывода чека возможно вводить в формате:

- для вывода в файл  _< output >-< Путь, имя файла >_

- для вывода в консоль  _< output >-< console >_ (для вывода в консоль данный параметр можно опустить)

> Пример:
> 
> - для вывода в файл, на диск <с:\check_out.txt>
> 
> _java CheckRunner  3-1 2-5 5-1 Card-123 output-_с:\check_out.txt__


> Пример:
> 
> - для вывода в консоль
> 
> _java CheckRunner  3-1 2-5 5-1 Card-123 output-console_

**Способ 2.** Передача параметров из файла.

Имя файла указываются в командной строке при запуске приложения в  формате  
_< file >-< Путь и имя файла >_

> Пример:
> 
> _java CheckRunner  file-D:\check.txt_

Параметры в файле аналогичны параметрам в способе 1. Параметры в файл заполняются одной строкой и разделяются пробелами.

> Пример:
> 
> - для вывода в  файл
> 
> _3-1 2-5 5-1_ _Card_-123 _output_-с:\
> 
> - для  вывода  в  консоль
> 
> _3-1 2-5 5-1 Card-123 output-console_

