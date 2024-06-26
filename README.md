# Parallelepiped task

В данном проекте вы напишите программу для вычисления некоторых величин, которые характеризуют такую геометрическую фигуру как параллелепипед. Это хороший кейс для обучения написанию скриптов.

**Параллелепипед** - это объемная фигура, каждой гранью которой является прямоугольником.

Если задан параллелепипед $ABCDA_1B_1C_1D_1$, то:

* $ABCD$, $\;\;\;AA_1B_1B$ ... - грани параллелепипеда
* $AB$ .. - ребра параллелепипеда.
* $d = AC_1 = A_1C = BD_1 = B_1D$ - главная диагональ параллелепипеда.

## From JSON

Вам предоставлен *json* файл `parallelepipeds.json`, который можете скачать [ТУТ](https://www.dropbox.com/scl/fi/yhqf1ebi17myh05ywa8so/parallelepipeds.json?rlkey=qypz0m2r0tslkqwmv8tqxh5jx&dl=0)

Его структура:



```
{
    "figure_1": {
        "a": "2",
        "b": "1",
        "c": "6"
    },
    "figure_2": {
        "a": "16",
        "b": "10",
        "c": "14"
    },
    "figure_3": {
        "a": "19",
        "b": "9",
        "c": "19"
    },
    ....,
}
```

Тут хранятся данные по 100 разным параллелепипедам, грани (длина, ширина и высота) $a$, $b$, $c$ каждого из которых находятся в словарях по ключам `figure_ ...` глобального словаря.

# Техническое задание для написания скрипта.

Напишите скрипт `my_first_script.py`, который можно запускать локально, который:

* Прочитает исходный `parallelepipeds.json`
* Сохранит в директорию два новых JSON файла
* "ЗАПРИНТИТ" сообщение о количестве фигур в файле в виде сообщения **`"Total number of figures <...count...>."`**
* В конце запринтит красиво полученные усредненные значения о которых пойдет речь далее.



