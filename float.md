# FLOATING POINT

## Common formats
|format    |ges. [bit]|Exponent [bit]|
|----------|----------|--------------|
|minifloat | 16       | 5            |
|binär     | 32       | 8            |
|binär 64  | 64       | 11           |
|double    | 64       | 7            |

## Getting started

(bsp.: minifloat)

10d in binär
<br>

## erster bit:
Der erste bit bestimmt das Vorzeichen.<br>
Daher sind auch zwei Nullen möglich.

daher ```0```

## exponenten bits:
Diese bits sind wichtig um zu ermitteln in welcher zweier potenz die zahl spielt.
es ist die höchste zahl beim convertieren.

nach bsp.:

10/2=5 R0<br>
5/2 =2 R1<br>
2/2 =1 R0<br>
1/2 =0 R1<br>
==> 1010

wenn dies als flieskommazahl dargestellt werden soll, steht bei den exponenten bits,<br>
die hochzahl der größten 1, sprich <b>2^3</b>.

da `10000`... immer `2^1` ist, ist 2^3= ```10010```.

## mantisse:

in der mantisse wird immer `2^n-1` gerechnet für jedes bit nach links.<br>
da im exponent ´1000 = 2^3´ dargestellt wurde, muss noch ´10 = 2^1´ dargestellt werden.<br>

da wir im exponenten 2 tiefer gehen muss unsere 1 die zweite stelle bei den mantissen bits sein.<br>
-> ```0100000000```

## zummenfassung:
```0 10010 0100000000```
das ist die zahl 10 in float darstellung.

daran sieht man auch das die genauigkeit von der höhe des ersten exponenten abhängt.
