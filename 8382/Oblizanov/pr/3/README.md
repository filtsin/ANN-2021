# Практическое задание №3, вариант 5

#### Входные данные:
Файл data.csv должен содержать 4 целых числа, разделенных пробелом. Программа распознает некорректные файлы и выводит сообщение об ошибке.

#### Функция chess_board
Функция принимает на вход 4 параметра: `m, n, a, b`.

* Создается матрица `m x n`, которая заполняется числами `a`. 

* С помощью обращения по наборам индексов осуществляется заполнение числами `b`:
  * четных элементов нечетных строк `[::2, 1::2]`
  * нечетных элементов четных строк `[1::2, ::2]`

Таким образом, получается шахматная доска из чисел `a, b`.

Результат сохраняется в файл `result.csv` в виде матрицы, разделенной пробелами, с помощью функции `np.savetxt`

#### Тестирование

Входные данные (10 строк, 20 столбцов, числа 6 и 9):
```
10 20 6 9
```
Выходные данные:
```
6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9
9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6
6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9
9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6
6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9
9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6
6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9
9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6
6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9
9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6 9 6
```


