# Задания на дом

## 2020-09-03

Дедлайн: 2020-09-10

### 0

- установить JDK, git
- создать **приватный** репозиторий 
  нужного формата
- задача 0 - программа выводит 
  `Hello world`

## 2020-09-08

Дедлайн: ~~2020-09-15~~ 2020-09-17

### 1

- ввести целые `x` и `y`
- вывести YES, если точка `(x,y)` находится в круге (граница принадлежит кругу)
  с радиусом 10, и NO иначе

### 2

- ввести целые `a` и `b`
- вывести периметр прямоугольника со сторонами `a` и `b`

## 2020-09-10

Дедлайн: 2020-09-17

### 3

- вводится `n`
- вводится `n` положительных целых чисел
- вывести сумму делителей этих чисел

```
3
1 4 5
14
```

В примере: `1+1+2+4+1+5`

### 4

- вводятся целые числа, ввод заканчивается, когда пользователь введёт `-1` (вводимых чисел не менее одного, пустых последовательностей чисел не будет)
- вывести минимальное число среди введённых

## 2020-09-15

Дедлайн: 2020-09-22

### 5

- вводится положительное целое число `n`
- вывести YES, если `n` представимо в виде суммы квадратов двух неотрицательных целых

```
25
YES
```

потому что `25 = 9 + 16`

```
10
YES
```

потому что `10 = 1 + 9`

```
7
NO
```

потому что `7 = 1 + 6 = 2 + 5 = 3 + 4`

### 6 

- вводится число `n`
- вводится `n` положительных целых чисел
- вывести `YES`, если все введённые числа ~~являются составными~~ не являются простыми

```
3
4 9 12
YES
```

```
4
4 3 6 9
NO
```

```
1
1
YES
```

потому что число 1 не является ни простым, ни составным

**UPD 2020-09-17.** Уточнено поведение на числе 1 (см. пример 3)

## 2020-09-17

Дедлайн: ~~2020-09-24~~ 2020-09-29.

### 7

- вводится число `n`
- вывести `YES`, если удвоенная сумма всех простых делителей числа больше `n`

```
14
YES
```

потому что `14 = 2 * 7 < 18 = 2*(2 + 7)`

```
18
NO
```

потому что `18 = 2*3^2; 2*(2+3) = 10 < 18`

### 8

- вводится число `n`
- вывести `YES`, если в разложении на простые делители `n` есть квадрат

```
30
NO
```

потому что `30 = 2*3*5`

```
24
YES
```

потому что `24 = 2^3 * 3`

### 9

- вводятся числа `n` и `k`
- проверить, что все простые делители `n` меньше `k`

```
98 10
YES
```

потому что `98 = 2 * 7^2` и `2 < 7 < 10`

```
77 10
NO
```

потому что `77 = 7 * 11` и `11 > 10`

```
13 13
NO
```

потому что 13 = 13 и 13 ≥ 13

## 2020-09-22

Дедлайн: 2020-09-29

### 10

Вводится последовательность целых чисел, ввод завершается `-1`.

Вывести сумму произведений троек соседних элементов (если меньше трёх элементов - выводится `0`).

```
1 2 3 -1
6
```

```
1 2 -1
0
```

```
1 2 3 4 -1
30
```

### 11

Вводится последовательность целых чисел, ввод завершается `-1`.

Вывести:
- символ `<`, если последовательность возрастает, 
- символ `>` - если убывает,
- символ `=` - если все элементы равны (включая случай, когда в последовательности меньше двух элементов),
- символ `!` - если последовательность не возрастает и не убывает (т.е. немонотонная). 

Сравнения нестрогие.

```
1 2 3 -1
<
```

```
3 2 1 -1
>
```

```
1 1 2 -1
<
```

```
2 2 1 -1
>
```

```
1 2 1 -1
!
```

```
1 1 1 -1
=
```

```
1 1 2 2 3 3 -1
<
```

```
1 1 2 2 1 1 -1
!
```

```
1 -1
=
```

```
-1
=
```

## 2020-09-24

Дедлайн: 2020-10-01

### 12

Вводятся целые числа, ввод завершается -1. Вывести сумму элементов между первым максимумом и последним минимумом (включая сами минимальный и максимальный элементы). Если максимум находится после минимума - ответ 0.

```
3 2 1 -1
6
```

```
3 2 5 2 1 -1
8
```

```
5 4 3 4 -1
12
```

```
5 4 3 4 1 -1
17
```

```
5 4 3 0 1 2 3 6 -1
0
```

```
5 3 5 3 1 3 1 -1
21
```

### 13

Вводятся целые числа, ввод завершается -1. Вывести второе по величине число (которое меньше максимального, но не меньше всех остальных). Если такого нет, вывести `NO`.

```
5 4 3 2 1 -1
4
```

```
5 5 4 3 2 -1
4
```

```
5 4 6 -1
5
```

```
5 -1
NO
```

```
5 5 -1
NO
```

```
-1
NO
```

## 2020-09-29

Дедлайн: 2020-10-06

### 14

Вводятся положительные целые числа, последовательность завершается -1.

Вывести максимальный элемент среди простых чисел в последовательности и сколько раз он встречается (или `NO`, если таких нет).

```
2 5 6 5 8 -1
5 2
```

```
1 6 8 -1
NO
```

### 15

Вводятся целые числа, последовательность завершается -1.

Вывести, сколько раз последовательность из неубывающей становится невозрастающей и наоборот.

```
1 2 3 2 1 -1
1
```

```
1 2 1 2 1 -1
3
```

```
1 2 2 1 -1
1
```

```
3 2 1 2 3 -1
1
```

```
2 2 2 2 -1
0
```

```
1 2 3 4 5 -1
0
```

```
5 4 3 2 1 -1
0
```

```
-1
0
```

```
1 -1
0
```
