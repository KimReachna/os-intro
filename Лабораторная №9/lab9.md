# РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ
## Факультет физико-математических и естественных наук
### Кафедра прикладной информатики и теории вероятностей

## ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ № 9
### *дисциплина: Операционные системы*

Студент: Ким Реачна
Группа: НПИбд-02-20

Москва
2021г.

---

### Цель работы:

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

### Теоретические сведения:

Редактор vi имеет три режима работы:

- командный режим — предназначен для ввода команд редактирования и навигации по редактируемому файлу

- режим вставки — предназначен для ввода содержания редактируемого файла

- режим последней (или командной) строки — используется для записи изменений
в файл и выхода из редактора

Для вызова редактора vi необходимо указать команду vi и имя редактируемого
файла: ```vi <имя_файла>```.

При этом в случае отсутствия файла с указанным именем будет создан такой
файл.

Переход в командный режим осуществляется нажатием клавиши ```Esc``` .

Для выхода из редактора vi необходимо перейти в режим последней строки: находясь в
командном режиме, нажать Shift-; (по сути символ : — двоеточие), затем:

- набрать символы wq, если перед выходом из редактора требуется записать изменения в файл

- набрать символ q (или q!), если требуется выйти из редактора без сохранения.

*Основные группы команд редактора*:

-  Команды управления курсором

- Команды позиционирования

- Команды позиционирования

-  Команды перемещения по файлу

- Команды перемещения по словам

- Команды редактирования: 
    - Вставка текста
    - Вставка строки
    - Удаление текста
    - Отмена и повтор произведённых изменений
    - Копирование текста в буфер
    - Вставка текста из буфер
    - Замена текста
    - Поиск текста

- Команды редактирования в режиме командной строки:
    - Копирование и перемещение текста
    - Запись в файл и выход из редактора

### Выполнение работы:

1. Ознакомиться с теоретическим материалом. [[1]](https://esystem.rudn.ru/pluginfile.php/1142371/mod_resource/content/2/006-lab_vi.pdf)
2. Ознакомиться с редактором ```vi```.
3. Выполнить упражнения, используя команды ```vi```.

***Задание 1. Создание нового файла с использованием vi***

1. Создайте каталог с именем ```~/work/os/lab09```:

*Рисунок 1: создание каталог ~/work/os/lab09*

![](https://sun9-18.userapi.com/impg/Iywh1s2MWaee2HoYBueFTcnAnkxJge5DvMxDkQ/YAU4fv7rRpY.jpg?size=527x179&quality=96&sign=a1fe6e701857fe50ae8c0c756a0efe96&type=album)

2. Перейдите во вновь созданный каталог ```~/work/os/lab09``` (*Рисунок 1*)

3. Вызовите vi и создайте файл ```hello.sh``` : ```vi hello.sh```: В работе здесь после того, как мы запустим команду ```vi hello.sh``` затем мы используем сочетание клавиш не работает для вставки текста, поэтому я установил VIM, чтобы решить проблему с помощью команды ```sudo apt-get install vim```

*Рисунок 2: вызов vi и создание файла hello.sh*

![](https://sun9-60.userapi.com/impg/v9afodzHREXyThkPycScC_BqF5PUT_vv9Utm-A/QlZSIkkYkww.jpg?size=492x69&quality=96&sign=22c4c065694f7bd6b08657d68c403445&type=album)

*Рисунок 3: Открыть файл hello.sh*

![](https://sun9-75.userapi.com/impg/APtOr9f0U4JP-PbhUGxl0ydBJOKQG_wQfA9cNw/hKDKvxuYIng.jpg?size=731x477&quality=96&sign=a2a53dc9e344c99bc8888ccf2ee9a099&type=album)

4. Нажмите клавишу``` i``` и вводите следующий текст.

*Рисунок 4: редактирование файла и ввод текста*

![](https://sun9-74.userapi.com/impg/7XPv9QsROzWdQcn1y_UnDTAGisxZ45wNz8Bzsw/xc-lsCb84uQ.jpg?size=727x478&quality=96&sign=ac89405f798b34d8393c2cc8e4474709&type=album)

5. Нажмите клавишу ```Esc``` для перехода в командный режим после завершения ввода
текста.

*Рисунок 5: нажмите клавишу Esc*

![](https://sun9-67.userapi.com/impg/oSwykSw16UvtXokElZZctqCNLhvsdHKtJBZprA/4ZHftIXTSdA.jpg?size=730x479&quality=96&sign=6b576898584f932984a24f339e93e24f&type=album)

6. Нажмите : для перехода в режим последней строки и внизу вашего экрана
появится приглашение в виде двоеточия. (*Рисунок 6*)

7. Нажмите ```w (записать) и q (выйти)```, а затем нажмите клавишу ```Enter``` для сохранения вашего текста и завершения работы.

*Рисунок 6: режим последной строки*

![](https://sun9-1.userapi.com/impg/aeocH8Zk2Bsn3aCMS_mRDsysG_Qj-4e0WFmv3A/ryg0XjM_w3g.jpg?size=730x477&quality=96&sign=c09f206cdef808d7b2d774ed17816c49&type=album)

8. Сделайте файл исполняемым : ```chmod +x hello.sh```

*Рисунок 7: делаем файл исполняемым*

![](https://sun9-63.userapi.com/impg/SBZV7qx2Up-CLyREI5igazpJDhfRAA0EIpZRDg/WER63VWMNB4.jpg?size=552x53&quality=96&sign=d6e55c45a22ee7ba4ca52136211c1b19&type=album)

***Задание 2. Редактирование существующего файла***

1. Вызовите vi на редактирование файла : ```vi ~/work/os/lab09/hello.sh```

*Рисунок 8: вызов vi на редактирование файла*

![](https://sun9-9.userapi.com/impg/ZmkR2G6V0_tx4uTOyIrc4RZFHrW4FMvtOtxmzw/ZmA74qiT9ws.jpg?size=619x47&quality=96&sign=9a3c1da4f7ac738159f4bbec56934ee6&type=album)

*Рисунок 9: вызов vi на редактирование файла*

![](https://sun9-4.userapi.com/impg/dESyLP7sDdp7yCmLJ9HyqVwD8ikg9Y8ns914fg/FvUcHpZd5tw.jpg?size=734x512&quality=96&sign=230a57fafb8230cf4bc61c951981cc3f&type=album)

2. Установите курсор в конец слова HELL второй строки

*Рисунок 10: Установите курсор в конец слова HELL*

![](https://sun9-23.userapi.com/impg/QsYDmRl9Kb8qBx_ka1vlIrnlnXWMOgBmemVx-A/Ojeqb4iYbes.jpg?size=738x274&quality=96&sign=42ee86420dd3fa27ba4c0c0b1c6ec868&type=album)

3. Перейдите в режим вставки и замените на HELLO. Нажмите ```Esc``` для возврата в
командный режим.

*Рисунок 11: замена HELL на HELLO*

![](https://sun9-32.userapi.com/impg/zN1i-wCCOCgBMhBEhxiqX7KlcMn5aK-oOMMCVQ/UkujSW1zst8.jpg?size=736x514&quality=96&sign=45b19d8e2a3e6cee4b11d70a397aa25a&type=album)

4. Установите курсор на четвертую строку и сотрите слово LOCAL : командой ```d+w```

*Рисунок 12: курсор на четвертую строку*

![](https://sun9-56.userapi.com/impg/Gypoq_MPtyVCdFNaWD8QSrQ_O52r8ohrle192g/DLLCVW5Jdvg.jpg?size=731x296&quality=96&sign=7b7224e25a318882adc2560c86a4252c&type=album)

*Рисунок 13: сотрите слово LOCAL*

![](https://sun9-23.userapi.com/impg/UsEPq0hJLXYiOzXmlj_OC8n8XyVy35Udt0FU3g/gByIifTa_-E.jpg?size=828x332&quality=96&sign=dcba287d5a1c7197f6d747ea97e4244c&type=album)

5. Перейдите в режим вставки ```i``` и наберите следующий текст: local, нажмите ```Esc``` для возврата в командный режим.

*Рисунок 14: ввод local*

![](https://sun9-6.userapi.com/impg/iqi3LWEma9CztPzq5psi83fjAh2BPwEmHaVRcQ/0Ey-TQu-sIU.jpg?size=730x510&quality=96&sign=135d32dc4edeb55196251ba837a2d3ef&type=album)

6. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую следующий текст: echo HELLO: Для этого мы сначала помещаем курсор на ```echo HELLO``` и копируем его с помощью команды ```Y``` (*рис. 15*), затем используем команду``` p```, которая позволяет вставлять текст, поэтому мы скопировали строку в конец текста (*рис. 16*)

*Рисунок 15: курсор на конец последней строки*

![](https://sun9-15.userapi.com/impg/D8E9LBBxcZClo9YXnG4eLLjgQ6PcM_I7TIk-pw/LK6ZRBtJzPI.jpg?size=733x245&quality=96&sign=c92a470cebb500d23b8225eaad8e5e6f&type=album)

*Рисунок 16: Скопируйте и вставьте строку*

![](https://sun9-75.userapi.com/impg/tbo2Osd6WlaU9hbwwpvaT04RTohwftIec4HWvQ/EEGbr4D9gR8.jpg?size=736x518&quality=96&sign=817b5553c2cd0556d242b0e45f75dd5f&type=album)

7. Нажмите ``` Esc``` для перехода в командный режим.

8. Удалите последнюю строку: Для этого мы используем команду ```dd``` для удаления строки.

*Рисунок 17: уделим последнюю строку*

![](https://sun9-17.userapi.com/impg/UJbsUfudD6ApPpx4MkGh8i9H9OJb4Nst2n9Dpw/y-NPcndc0Sw.jpg?size=738x413&quality=96&sign=b99032770c104c15f25b6e2cb469cdb4&type=album)

9. Введите команду отмены изменений ```u``` для отмены последней команды.

*Рисунок 18: отмены последней команды*

![](https://sun9-75.userapi.com/impg/tbo2Osd6WlaU9hbwwpvaT04RTohwftIec4HWvQ/EEGbr4D9gR8.jpg?size=736x518&quality=96&sign=817b5553c2cd0556d242b0e45f75dd5f&type=album)

10. Введите символ ```:``` для перехода в режим последней строки , мы используем команды ```w(запись) и q(выход)``` после ```:``` (*Рисунок 19*) и нажимаем ```Enter```. Запишите произведённые изменения и выйдите из ```vi``` (*Рисунок 20*).

*Рисунок 19: режим последней строки*

![](https://sun9-15.userapi.com/impg/QuYYlex0OAszGzSUU8ZPHb0tJE9ty8sDEvNCAA/VMSyoGjlxJE.jpg?size=742x518&quality=96&sign=5bf7a2036a2ad5de7d5ee15147559f28&type=album)

*Рисунок 20: выйдите из ```vi```*

![](https://sun9-17.userapi.com/impg/cVtdPpaAMYU6iS6D9iLSS06odBEvLMxzKcQVTg/43YGqaf-Wkk.jpg?size=738x513&quality=96&sign=991bf7bf876500df499fc47847335a04&type=album)

### Вывод:

Я познакомилась с операционной системой Linux. Получила практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах

#### Библиография:

[1][Лабораторная работа №9](https://esystem.rudn.ru/pluginfile.php/1142371/mod_resource/content/2/006-lab_vi.pdf)