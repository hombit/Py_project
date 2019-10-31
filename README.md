# Py_project

Мой проект по сути - кусочек курсовой, мне надо тут все оптимизировать и в итоге написать скрипт, или даже может сделать какой-то удобный интерфейс для общения с программой (я пока не умею это делать, поэтому пока будет просто программа на питоне).

В чем суть работы: у меня есть 4D сетка данных, зависимость показателей цвета (раличных) от эффекивной температуры, log(g) и [Fe/H] (все заданно с определенным шагом). Нужно сделать так, что-бы любой челоек, мог по своим значениям металличности и логарифма g и зная показатель цвета определить температуру звезды. (Т.е необходимо получить промежуточные значения для сетки - либо аппроксимацией, либо интерполяцией.) Я выбрала двумерную интерполяцию, т.к. апрокимация для данного вида зависимости не очень хорошо подходила.

Пока у меня есть только сама интерполяция, и написана она не очень хорошо. Я хочу поправить эту программу с помощью масок для массивов (для выбитых точек) и др.


В первом варианте кода представлена реализация двумерной интерполяции для 11 различных значений log(g) (от 0 до 5 с шагом 0.5), т.е. строится зависимость эффективной температуры от показателя цвета J-K и [Fe/H].

argparce
