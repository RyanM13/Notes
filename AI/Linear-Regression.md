# Linear Regression

- Very -very basic form of prediction
- You are going to have a set of samples, about something
  | Names |
  | ------------- |
  | Phenomena |
  | Occurence |
  | Experiment|
  | Event |

- The set of sameples will be given in a group of (x,y) pair, values.
- X is known as the Independent variable (Does not depend on anything)
- Y is known as the Depenendent variable the value of y, will depend on x and some other info.

### Sample Acquisition

Apply Linear Regression -> to get a model

- A model that will allow me to make predictions about a possible outcome given some expected conditions.
- Model (on a graph) gives you a line

| x          | y          |
| ---------- | ---------- |
| horizontal | horizontal |
| value      | value      |
| value      | value      |
| value      | value      |
| vertical   | vertical   |

- Linear implies == y = mx + b

### Structure

- m = slope
- b = y intercept, value y takes when x = 0, units b[y-units]
- m = y/x, unit m[y units/x units]
- N = # of samples, # of (x,y) pairs.

- M = N * $$\sum_$$ (x*y) - ($$\sum$$x) _ ($$\sum$$y)/ N _ $$\sum$$(x^2) - ($$\sum$$x)^2

| x(hours of sunshine) | y(ice cream sold) |
| -------------------- | ----------------- |
| 2                    | 4                 |
| 3                    | 5                 |
| 5                    | 7                 |
| 7                    | 10                |
| 9                    | 15                |

Do linear regression to find model now.

Steps

- Step 1 (table) x, y
- | x(hours of sunshine) | y(ice cream sold) | X^2 | XY  |
  | -------------------- | ----------------- | --- | --- |
  | 2                    | 4                 | 4   | 8   |
  | 3                    | 5                 | 9   | 15  |
  | 5                    | 7                 | 25  | 35  |
  | 7                    | 10                | 49  | 70  |
  | 9                    | 15                | 81  | 135 |

  - Step 2

  | Sum | Sum x | SUm y | sum x^2 | sum (xy) |
  | --- | ----- | ----- | ------- | -------- |
  |     | 26    | 41    | 168     | 263      |

- step
  compute the slope

m = (5 _ 263) - (26) _ (41) / (5 \* 168) - (26)^2

m = 1315 - 1066 / 840 - 676 = 249/164= 1.51829268293

ice cream sold/ hours of sunshine = y/x = x2 - x1 / y2 - x1

- Step 4 compute b

- b = sum y - m times sum x / N
  = 41 - (1.51829268293)
  = 31 - 39.4756097562 / 5

- 1.5283802433 / 5
- b = 0.30487804876 [ice cream sold]

- Step 5
- put together the elements that will give you the model that describes the system by

x = 8
y = 1.51829268293 times x + 0.30487804876
12.1463414643 + 0.30487804876

y = 12.4512195122 [Ice creams sold]

## Corelation coefficient

- Step 6 How good is the model?

r = N _ (SumXY) - (SumX)(SumY) / rad[N_(SumX^2)-(SumX)^2] _ rad[N_(SumY^2)-(SumY)^2]

- | x(hours of sunshine) | y(ice cream sold) | X^2 | XY  | y   |
  | -------------------- | ----------------- | --- | --- | --- |
  | 2                    | 4                 | 4   | 8   | 16  |
  | 3                    | 5                 | 9   | 15  | 25  |
  | 5                    | 7                 | 25  | 35  | 44  |
  | 7                    | 10                | 49  | 70  | 100 |
  | 9                    | 15                | 81  | 135 | 225 |

  | Sum | Sum x | SUm y | sum x^2 | sum (xy) | Sum Y |
  | --- | ----- | ----- | ------- | -------- | ----- |
  |     | 26    | 41    | 168     | 263      | 415   |

  r = 5 _ (263) - (26)(41) / rad[(5 _ 168) - (26)^2] * rad[(5 *415) - (41)^2]

  r = 1315 - 1066 / rad[840 - 676] \* rad[2075 - 1681]

  r = 244 / rad[164] \* rad[399] = 249 / 254.1967
  r = 0.97556097079

r =

| -1        | 0                            | 1              |
| --------- | ---------------------------- | -------------- |
| exact fit | no fit at all                | exact fit      |
| trustable | no linear correlatoin at all | trustable 100% |

- As r approaches zero the linear association/correlatoin decreases.

- under 0.80 don't trust very much. Maybe even 0.85
