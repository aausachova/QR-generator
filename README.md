# QR-generator

## Задача:
Разработать программу для генерации подарочных сертификатов

## ОС: Windows 7,8,10
Формат: Приложение .exe

## Функционал:
Циклическая функция, создающая одно изображение за цикл из двух других

До выполнения цикла приложение последовательно запрашивает от пользователя ввод с клавиатуры:

•	«Количество генерируемых сертификатов» - число в диапазоне от 1 до 100000 (Vmax)

•	«Порядковый номер первого штрихкода» - число в диапазоне от 1 до 100000 (Nstart)

В течение цикла:

•	Присвоить переменной счетчика циклов начальное значение V=1, а переменной номера штрихкода начальное значение N=Nstart

•	Взять изображение фона сертификата – файл bgr.jpg из папки, где находится приложение. Изображение имеет размер 1280*598 пикселей, вертикальное расположение. Вместо файла bgr.jpg можно использовать файл bgr.gif при необходимости.

•	Взять из папки, где находится приложение, изображение штрихкода с порядковым номером N и разместить его поверх изображения bgr так, чтобы верхняя левая точка изображения со штрихкодом была в координате Х=144 , Y=765 пикселей. Наименование файлов со штрих-кодами имеет формат «N_Z.gif», где N – порядковый номер штрихкода, Z – цифробуквенная строка, закодированная в штрихкоде, длина которой может быть от 6 до 20 символов (тестовые штрихкоды содержат 18 символов). Размер изображения со штрихкодом 312*100 пикселей (горизонтальное)

•	Сохранить полученное изображение, состоящее из фона и одного штрихкода, в папке, где находится приложение с именем «N_sertif.???» формате jpg (предпочтительно) или gif. N в имени файла – цифра, соответствующая порядковому номеру штихкода (цифра до «_» в название файла)

•	Прибавить единицу к значению переменной V

•	Прибавить единицу к значению переменном N

•	Закончить программу, если V превысит Vmax


## Обязательные условия:

•	Приложение должно запускаться процедуры установки и без доступа к интернету

•	Приложение не должно передавать какие-либо данные на внешние адреса/компьютеры

•	Все временные файлы должны сохраняться исключительно в папке нахождения Приложения.

