# if (a-b)>0: answer = 1 else: 0
как мат-операциями избежать условия если для условия темы
Пример задачи, где используется:
Формат входных данных
Вводится ﻿44﻿ целых положительных числа ﻿A,B,C,D(1≤A,B,C,D≤100)A,B,C,D(1≤A,B,C,D≤100)﻿ — стоимость тарифа Кости, размер тарифа Кости, стоимость каждого лишнего мегабайта, размер интернет-трафика Кости в следующем месяце. Числа во входном файле разделены пробелами.

Формат выходных данных
Выведите одно натуральное число — суммарные расходы Кости на интернет.

Замечание
В примере Костя сначала оплатит пакет интернета, после чего потратит на ﻿55﻿ мегабайт больше, чем разрешено по тарифу. Следовательно, за ﻿55﻿ мегабайт он дополняет отдельно, получившаяся стоимость ﻿100+12×5=160100+12×5=160﻿ рублей.

Ввод: 100  10  12  15

Вывод: 160

Решение:
``` Python 
a,b,c,d=map(int,input().split())
print(c*(d-b)*((d//b)//(d//b-0.4))+a)
```
