#### Ивницкий Алексей, M3205
## Лабораторная работа №6

Вычислить значение производной функции $f(x) = \frac{1}{1 + sin(x)}$ в точке х = 1.5
C помощью полинома Ньютона и шага 0.25 на промежутке [1;2]

C помощью полинома Ньютона:
```C
double t = (x - from) / h;
var y = new double[5, 5];
for (var i = 0; i < 5; i++)
    y[0, i] = f(from + h * i);
for (var i = 1; i < 5; i++)
    for (var j = 0; j + i < 5; j++)
        y[i, j] = y[i - 1, j + 1] - y[i - 1, j];
double ans = 1 / h
* (y[1, 0]
    + (2 * t - 1) / 2 * y[2, 0]
    + (3 * t * t - 6 * t + 2) / 6 * y[3, 0]
    + (4 * t * t * t - 18 * t * t + 22 * t - 6) / 24 * y[4, 0]);

return ans;
```
```C
double y1 = f(1.5 + h);
double y2 = f(1.5 - h);
double res = (y1 - y2) / (2 * h);
return res;
```

$$
y = 4.78748,  
y_1 = 4.78995 (\delta = 0.00247),
y_2 = 4.78748
$$