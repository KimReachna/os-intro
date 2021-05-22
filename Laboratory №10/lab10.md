# РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ
## Факультет физико-математических и естественных наук
### Кафедра прикладной информатики и теории вероятностей

## ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ № 10
### *дисциплина: Операционные системы*

Студент: Ким Реачна
Группа: НПИбд-02-20

Москва
2021г.

---

### Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs. 

### Теоретические свдения:

Emacs представляет собой мощный экранный редактор текста, написанный на языке высокого уровня Elisp.

**Основные термины Emacs**

*Буфер* — объект, представляющий какой-либо текст.

*Фрейм* соответствует окну в обычном понимании этого слова. Каждый фрейм содержит область вывода и одно или несколько окно Emacs.

*Окно* — прямоугольная область фрейма, отображающая один из буферов.

*Область вывода* — одна или несколько строк внизу фрейма, в которой Emacs выводит различные сообщения, а также запрашивает подтверждения
и дополнительную информацию от пользователя.

*Минибуфер* используется для ввода дополнительной информации и всегда отображается в области вывода.

*Точка вставки* — место вставки (удаления) данных в буфере.


**Основы работы в Emacs**

Для запуска Emacs необходимо в командной строке набрать emacs (или emacs & для работы в фоновом режиме относительно консоли). 

Для работы с Emacs можно использовать как элементы меню, так и различные сочетания клавиш. Например, для выхода из Emacs можно воспользоваться меню ```File``` и выбрать пункт ``` Quit``` , а можно нажать последовательно ```Ctrl-x Ctrl-c ```(в обозначениях Emacs:``` C-x C-c```).

По назначению префиксные сочетания клавиш различаются следующим образом:

- ```C-x``` — префикс ввода основных команд редактора (например, открытия, закрытии, сохранения файла и т.д.);

- ```C-c``` — префикс вызова функций, зависящих от используемого режима.

*Режим* — пакет расширений, изменяющий поведение буфера Emacs при редактировании и просмотре текста (например, для редактирования исходного текста программ на языках С или Perl). 

Более подробная ссылка на материал[[1]](https://esystem.rudn.ru/pluginfile.php/1142374/mod_resource/content/3/007-lab_emacs.pdf) [[2](https://www.gnu.org/s/emacs/manual/html_node/emacs/Term-Mode.html)]

### Выполнение работы:

1. Открыть emacs: Чтобы открыть Emacs , мы используем команду ```emacs```, так как у меня нет Emacs, поэтому мне нужно сначала установить его с помощью команды ```sudo snap install emacs --classic``` *(Рисунок 1)*, после завершения установки снова запустите команду ```emacs```, мы увидим редактор окон *(Рисунок 2)*. 

*Рисунок 1:Установка emacs*

![](https://sun9-51.userapi.com/impg/ygVbD1NM8Q9SOLUH1n7bT5V1X_tLnX3o_JuWTw/Zt2IOli3nnI.jpg?size=727x435&quality=96&sign=e49f51135abc466b4a82e4f66b44812b&type=album)

*Рисунок 2: открываем редактор Emacs*

![](https://sun9-25.userapi.com/impg/qn5aLRQd6P2sko4tEdv5HfXpV67Gu8h3rKDftw/YDTOpM_rkWc.jpg?size=1106x649&quality=96&sign=043736524ad3a71b1bd4c4070454ba90&type=album)

2. Создать файл lab10.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

*Рисунок 3: Создать файл lab10.sh*

![](https://sun9-62.userapi.com/impg/g5XimVa3EUimoQRrmo8H7gdX_nH_KDGKjGPsrg/GjftyC93gRk.jpg?size=756x164&quality=96&sign=ac9f305abad104eb9eb0961f78bc73c6&type=album)

*Рисунок 4: Файл lab10.sh*

![](https://sun9-3.userapi.com/impg/y8brJ9H5vRRuuvtSKXmLjJCqg2CPuYWjV-zagA/NFgj0-c6ngY.jpg?size=754x478&quality=96&sign=3251c355340071791893a06847d07552&type=album)

3. Наберите текст:

```
#!/bin/bash
HELL=Hello
function hello {
    LOCAL HELLO=World
    echo $HELLO
}
echo $HELLO
hello
```

*Рисунок 5: набор текста*

![](https://sun9-53.userapi.com/impg/_bAJUX5XtSHJMJR16oi2SbcVQVRkDKTGH8taJg/exg-e_ifzPA.jpg?size=752x475&quality=96&sign=a96c58c1408be96ed79390beecf4fd82&type=album)

4. Сохранить файл с помощью комбинации ```Ctrl-x Ctrl-s (C-x C-s).```

*Рисунок 6: Сохранить файл*

![](https://sun9-16.userapi.com/impg/FQBzylnsqaZO0knPpjlQxG9eOwDN5d0D2YSSKQ/mp6hJbvUM2M.jpg?size=754x475&quality=96&sign=88f41c893eb84fc4aa6dcfa57e7db97c&type=album)

5. Проделать с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш:

    5.1. Вырезать одной командой целую строку ```С-k```: сначала мы выбираем строку , которую хотим выстроить, выбираем с самого начала *(Рисунок 7)* , а затем используем команду ```C - k```, чтобы вырезать строку (*Рисунок 8*).

    *Рисунок 7: Выберите строку,которую мы хотим вырезать*

    ![](https://sun9-24.userapi.com/impg/UaUc-gmGrI4d_aZ97UgjOihjxvpAjAEc45IubA/qWvPCGEKI1A.jpg?size=751x477&quality=96&sign=11960e609f8a6013169bba87baa08690&type=album)

    *Рисунок 8:используйте ```C -k```, чтобы обрезать строку*

    ![](https://sun9-15.userapi.com/impg/Sm-eq_lbw_ArFbuNdwMm3t_8va6yIAN-xHW1IQ/hZsI0kJ4PYo.jpg?size=749x477&quality=96&sign=ed05f95eaf511815f271bb7025dc2a97&type=album)

    Как мы видим, четвертая строка успешно обрезана. 

    5.2. Вставить эту строку в конец файла ```C-y```: для этого мы переходим в конец файла, а затем используем команду ```C - y```, чтобы вставить эту строку (*Рисунок 9*)

    *Рисунок 9:Вставить эту строку в конец файла*

    ![](https://sun9-24.userapi.com/impg/D0QId_JkQF1d3F2WX7uodEAkmz7YXK4F_O3j5g/K6qVEMwa7iE.jpg?size=752x480&quality=96&sign=fbcaf49409352bce02b5201242e2cae4&type=album)

    5.3. Выделить область текста ```C-space```:В работе я выбираю третью строку и использую ```C - space```, а затем использую клавишу со стрелкой до конца строки, а затем использую ```M - w```, чтобы скопировать выбранную нами строку (*Рисунок 10*). 

    *Рисунок 10: Выделить область текста (C-space) и M-w для копирования*

    ![](https://sun9-24.userapi.com/impg/bYvRlKRWH0BJDuK8hKMOqaIANsdav7zp8F1ysw/tNqvd_rd8JY.jpg?size=751x473&quality=96&sign=2d58fee2b5be5daed678baaca2ce5474&type=album)

    5.4. Скопировать область в буфер обмена ```M-w``` (*Рисунок 10*).

    5.5. Вставить область в конец файла: для этого мы снова переходим к концу файла, а затем используем ```C-y``` для вставки (*Рисунок 11*).

    *Рисунок 11: Вставить область в конец файла*

    ![](https://sun9-42.userapi.com/impg/doTQBkkRre8he6VoA2LC28eOKQ8j6SmrGRlSMw/lvP643hiP4o.jpg?size=755x391&quality=96&sign=b8597c2534b490d3a168293e18120d5b&type=album)

    5.6. Вновь выделить эту область ```C - space``` (*Рисунок 12*) и на этот раз вырезать её ```C - w``` (*Рисунок 13*)

    *Рисунок 12: выделить область*

    ![](https://sun9-44.userapi.com/impg/iQJrrcrERDnIbnenoBsUBJasiVt_pV1rb3cxMw/DgwPCViXgKs.jpg?size=752x392&quality=96&sign=8ba6151e9bd8605b7678f355dd3cd3fc&type=album)

    *Рисунок 13: вырезка текста*

    ![](https://sun9-45.userapi.com/impg/cRqyFDVEAczs_3dzI-lJaKkgxsyi7PBi6EWDQA/QH1Kx7wrxG4.jpg?size=753x390&quality=96&sign=a473b39222a38d481490f4d40618483d&type=album)

    5.7. Отмените последнее действие ```C - /``` (*Рисунок 14*)

    *Рисунок 14: Отмените последнее действи*

    ![](https://sun9-11.userapi.com/impg/0Rl_UyScDY5kxbQTVs_eDB6-3eCgJPJT347zaQ/YMRKr67uNY4.jpg?size=753x390&quality=96&sign=b1fc1addef5af84dbeb0957e7ede7035&type=album)

    Как мы видим, текст возвращается обратно. 

6. Научитесь использовать команды по перемещению курсора. 

    6.1. Переместите курсор в начало строки ``` C - a```(*Рисунок 15*) : как мы видим начальное положение курсора на (*рисунке 14*).

    *Рисунок 15: Переместите курсор в начало строки*

    ![](https://sun9-58.userapi.com/impg/Zt-pjFlXGqgyoFEVorYEUPHEymOo0P3VSiEyTQ/E2fm4TR0QSs.jpg?size=750x390&quality=96&sign=138d7e0733a89586d7e95fde5cbc1e7f&type=album)

    6.2. Переместите курсор в конец строки ```C-e``` (*Рисунок 16*)

    *Рисунок 16: Переместите курсор в конец строки*

    ![](https://sun9-42.userapi.com/impg/yYluI-YjbOs0Fk3BBInce7Ys7IE7Tfy6vtA2uQ/o_Phgl9vPQ8.jpg?size=662x246&quality=96&sign=16307e5ebb2a40a9d67d55e76f0b2aa8&type=album)

    6.3. Переместите курсор в начало буфера ```M - <```. (*Рисунок 17*)

    *Рисунок 17: Переместите курсор в начало буфера*

    ![](https://sun9-4.userapi.com/impg/gk-Mmkrpl1FephlRHeAAjlWo7eznHhadjSY4_A/CfIfydpyMnI.jpg?size=754x385&quality=96&sign=3021594bc7a14ce37d34626d73054e34&type=album)

    6.4. Переместите курсор в конец буфера ```M - >```. (*Рисунок 18*)

    *Рисунок 18: Переместите курсор в конец буфера*

    ![](https://sun9-17.userapi.com/impg/DKPs2bXVA4gzHp-C65sWgzA2IRV9dRFOeVnP1w/AMrckYnk2A0.jpg?size=755x386&quality=96&sign=29fe05586daff8588b7f6fdbacd92eb1&type=album)

7. Управление буферами.

    7.1. Вывести список активных буферов на экран ```C-x C-b``` (*Рисунок 19*)

    *Рисунок 19: Вывести список активных буферов*

    ![](https://sun9-45.userapi.com/impg/Cc09qiALuvbhTya5uoCf48P7mJGAckwtc_ZMQw/dqpEvqGzNj0.jpg?size=665x679&quality=96&sign=5bae2bee68ab4d4c54225b7174d13dbe&type=album)

    7.2. Переместитесь во вновь открытое окно ```C-x o``` (*Рисунок 20*) со списком открытых буферов и переключитесь на другой буфер ```C-x b``` (*Рисунок 21*)

    *Рисунок 20: Переместитесь во вновь открытое окно*

    ![](https://sun9-55.userapi.com/impg/Posu2WvUPJ3KuZ5WnvkZhnH4uLuo4u8OtT2o7A/1W81SAaH7RY.jpg?size=662x675&quality=96&sign=dcb5a1f40f8088cf11578a78bfdeadf1&type=album)

    *Рисунок 21: переключитесь на другой буфер*

    ![](https://sun9-74.userapi.com/impg/d-OY4ZPElSBPXZOAaitwh66BJaUv6bGOSf_FnQ/h7vhpaTHZZ8.jpg?size=660x673&quality=96&sign=d3205a66ec3ff77f40cd3c1b32abc0db&type=album)

    7.3. Закройте это окно ```C-x 0``` (*Рисунок 22*).

    *Рисунок 22: Закройте окно*

    ![](https://sun9-63.userapi.com/impg/w99THQlIQNwcHYBp4_djqSF8EDDrwyhLeqKSOg/TTd4OsxAvxU.jpg?size=662x546&quality=96&sign=405eaa6d748c9c335a5178ef6720265a&type=album)

    7.4. Теперь вновь переключайтесь между буферами, но уже без вывода их списка на экран ```C-x b```(*Рисунок 23*).

    *Рисунок 23: вновь переключайтесь между буферами*

    ![](https://sun9-54.userapi.com/impg/SNJBWRZk8W7Aet9nLDwB5yc8g_Mc6cHMFYbRpw/XnULsYVxUFE.jpg?size=660x550&quality=96&sign=5da8daa5d7fe61ec10a4d3a06db4a87a&type=album)

8. Управление окнами.

    8.1. Поделите фрейм на 4 части: разделите фрейм на два окна по вертикали ```C-x 3```(*Рисунок 24*), а затем каждое из этих окон на две части по горизонтали ```C-x 2```(*Рисунок 25*). 

    *Рисунок 24: деление окна по вертикали*

    ![](https://sun9-58.userapi.com/impg/wZh0hMYsWm3FMZ8zXtVrke3hioJ1L8ojgW4N8g/FDmuvKVFYTU.jpg?size=663x548&quality=96&sign=31b293d3276c30b121ab188c0bfd0a19&type=album)

    *Рисунок 25: деление окна по вертикали*

    ![](https://sun9-35.userapi.com/impg/sxDaU-ZtrBzcjX-f2yfsgJ4gZLXr6f2qSJJqCg/2s2tm7MGNiQ.jpg?size=664x546&quality=96&sign=bc8e5ca00e36edfa3c048bc44f56a16d&type=album)

    8.2. В каждом из четырёх созданных окон откройте новый буфер (файл) new_file.txt ```C-x C-f``` (*Рисунок 26-27*) и введите несколько строк текса (*Рисунок 28*)

    *Рисунок 26: открытие файла во всех окнах*

    ![](https://sun9-61.userapi.com/impg/bnmQYqhjx_lllD_dFaDSDJN01EhN0OptZfia_g/FYWf7heM_J0.jpg?size=662x547&quality=96&sign=cedf945c1945570b842f9673fb15d1cb&type=album)

    *Рисунок 27: открытие файла во всех окнах*

    ![](https://sun9-67.userapi.com/impg/R2qFdPGizDIZkDfoMxOt_3TdtadQogear5kCGA/JqUfEaYzuKA.jpg?size=664x550&quality=96&sign=49d0a3a1c28d72e7c868e843daea543a&type=album)

    *Рисунок 28: ввод текста*

    ![](https://sun9-38.userapi.com/impg/m8Cw3W72C2lAYLn4p9_Ih3RYxeWCpisNWjFIiQ/CjoVi7cr5s8.jpg?size=663x545&quality=96&sign=1e2911ad533d7b6bcdf00a816406f36d&type=album)

9. Режим поиска

    9.1. Переключитесь в режим поиска ```C-s```(*Рисунок 29*) и найдите несколько слов (*Рисунок 30*), присутствующих в тексте. 

    *Рисунок 29: Переключитесь в режим поиска ```C-s```*

    ![](https://sun9-8.userapi.com/impg/OCV_wPdMObDLMSIY_9ZPRUk1C60iDY7Tcxve4Q/FbFOGR4sFGc.jpg?size=661x545&quality=96&sign=348d913a63a26cb45319c9cab02da919&type=album)

    *Рисунок 30: найдите несколько слов (file)*

    ![](https://sun9-1.userapi.com/impg/3Z8OjBv-CKwzCY7N9nbacIMM6E3pqFRG_JL_Pg/t5ItzOKj5P8.jpg?size=662x549&quality=96&sign=a7c43d1d3046fce2a0d645fcfc4ccdaf&type=album)

    9.2. Переключайтесь между результатами поиска, нажимая ```C-s``` (*Рисунок 31-32*)

    *Рисунок 31: Переключайтесь между результатами поиска*

    ![](https://sun9-1.userapi.com/impg/N3ZqhRM389P0rtttNKG2RDdHqrH4ooKFEy7Vuw/NsU_Xwr3oTs.jpg?size=665x551&quality=96&sign=cddb01a4333252358da3576685de3f40&type=album)

    *Рисунок 32: Переключайтесь между результатами поиска*

    ![](https://sun9-42.userapi.com/impg/_CoYi-eCFQVuwoD5-6QXH9AZoCfvYD34LbbQtg/CPA5c-7XzcI.jpg?size=662x543&quality=96&sign=e29c5c1c031e6529c4910875835a4d3a&type=album)

    9.3. Выйдите из режима поиска, нажав ```C-g``` (*Рисунок 33*)

    *Рисунок 33: Выйдите из режима поиска*

    ![](https://sun9-41.userapi.com/impg/rzjoWO8OhfQ03GmcIV8RJYOKmhzx3EQV0roBqQ/ZJOFT-OViak.jpg?size=664x546&quality=96&sign=19f77ca97cca95bdd0c83f88edace54d&type=album)

    9.4. Перейдите в режим поиска и замены ```M - %```, введите текст, который следуетнайти и заменить, нажмите ```Enter``` , затем введите текст для замены. После того как будут подсвечены результаты поиска, нажмите ! для подтверждения замены

    *Рисунок 34: Замените слово LOCAL на FILE и результаты* 

    ![](https://sun9-51.userapi.com/impg/4Q2Xym51H_ykhVottOnfkAl8TSrQynxhWGPyzQ/PURif1PebJI.jpg?size=661x547&quality=96&sign=1f5317fdb801b87bf4e469825687fe27&type=album)

    *Рисунок 35: Замена*

    ![](https://sun9-55.userapi.com/impg/enK2BQktkeoTUoCj_rstvyckXN72Jy85eal1cg/mYjq4LoZBnE.jpg?size=662x548&quality=96&sign=46bc515c3baaa87b7e42bd0a4bdd121f&type=album)

    9.5. Испробуйте другой режим поиска, нажав ```M-s o``` в этом мы ищем слово hello, так как видим, что оно ищет не введенное слово, а строку, в которой оно встречается (*Рисунок 36*). 

    *Рисунок 36:Испробуйте другой режим поиска M-s o*

    ![](https://sun9-33.userapi.com/impg/Tp23XDGyVhEgqvW7pb4tj58mbaKnQ5RfAmCIqg/ZC6AEhM71bc.jpg?size=663x549&quality=96&sign=cd560093a8defea49ae81dd009166e42&type=album)

---

### Вывод: 

Я познакомилась с операционной системой Linux. Получила практические навыки работы с редактором Emacs. 

#### Библиография:

[1] [Лабораторная №10](https://esystem.rudn.ru/pluginfile.php/1142374/mod_resource/content/3/007-lab_emacs.pdf) 
[2] [Термин Emacs](https://www.gnu.org/s/emacs/manual/html_node/emacs/Term-Mode.html)


