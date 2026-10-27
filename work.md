# Вариант 6: решения задач

## Задача 1
**Дано:** $(X > 2) \vee (X < 2) \vee (X > 4)$, $X = 4$.  
**Решение:**  
- $X > 2 \Rightarrow 4 > 2 \Rightarrow \text{истина}$;  
- $X < 2 \Rightarrow 4 < 2 \Rightarrow \text{ложь}$;  
- $X > 4 \Rightarrow 4 > 4 \Rightarrow \text{ложь}$;  
- $\text{истина} \vee \text{ложь} \vee \text{ложь} = \text{истина}$.  
**Ответ:** $1$.

---

## Задача 2

- Прямая $l$.
- Плоскость $\pi$.
- Прямые $a$, $b$, $c$ лежат в плоскости $\pi$ ($a, b, c \subset \pi$).
- $l \perp a$ (прямая $l$ перпендикулярна прямой $a$).
- $l \perp b$ (прямая $l$ перпендикулярна прямой $b$).
- $l \not\perp c$ (прямая $l$ не перпендикулярна прямой $c$).

Требуется доказать: $a \parallel b$ (прямые $a$ и $b$ параллельны).


Если бы прямые $a$ и $b$ пересекались, то по признаку перпендикулярности прямой и плоскости следовало бы $l \perp \pi$. Но тогда $l$ была бы перпендикулярна любой прямой в плоскости — в том числе и $c$. Это противоречит условию $l \not\perp c$, значит, $a$ и $b$ не пересекаются.  

Так как $a$ и $b$ лежат в одной плоскости и не пересекаются, они параллельны: $a \parallel b$.  

**Ответ:** утверждение истинно.


---

## Задача 3
**Дано:** $(Y \vee Z \leftrightarrow X) \vee ((X \rightarrow Y) \vee Z)$.  
**Решение:**  
- $X \rightarrow Y = \overline{X} \vee Y$;  
- $(\overline{X} \vee Y) \vee Z = \overline{X} \vee Y \vee Z$;  
- $Y \vee Z \leftrightarrow X = ((Y \vee Z) \wedge X) \vee (\overline{Y} \wedge \overline{Z} \wedge \overline{X})$;  
- Итоговое выражение: $((Y \vee Z) \wedge X) \vee (\overline{Y} \wedge \overline{Z} \wedge \overline{X}) \vee \overline{X} \vee Y \vee Z$;  
- $\overline{X} \vee Y \vee Z$ делает выражение истинным при всех значениях переменных.  
**Ответ:** $1$.

---

## Задача 4
**Дано:** $\overline{(A \vee B)} \vee (\overline{B} \wedge A)$.  
**Решение:**  
- $\overline{(A \vee B)} = \overline{A} \wedge \overline{B}$;  
- $(\overline{A} \wedge \overline{B}) \vee (\overline{B} \wedge A) = \overline{B} \wedge (\overline{A} \vee A) = \overline{B} \wedge 1 = \overline{B}$.  
**Ответ:** $\overline{B}$.

---

# Задача 5: построение таблицы истинности

**Дано:** $((\overline{X} \leftrightarrow \overline{Y}) \rightarrow (Y \wedge X)) \vee (X \rightarrow Y)$

| $X$ | $Y$ | $\overline{X}$ | $\overline{Y}$ | $\overline{X} \leftrightarrow \overline{Y}$ | $Y \wedge X$ | $(\overline{X} \leftrightarrow \overline{Y}) \rightarrow (Y \wedge X)$ | $X \rightarrow Y$ | $((\overline{X} \leftrightarrow \overline{Y}) \rightarrow (Y \wedge X)) \vee (X \rightarrow Y)$ |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 0   | 0   | 1   | 1   | 1               | 0              | 0                                             | 1              | 1                                                                                               |
| 0   | 1   | 1   | 0   | 0               | 0              | 1                                             | 1              | 1                                                                                               |
| 1   | 0   | 0   | 1   | 0               | 0              | 1                                             | 0              | 1                                                                                               |
| 1   | 1   | 0   | 0   | 1               | 1              | 1                                             | 1              | 1                                                                                               |

**Финальный ответ:** $1$ (тождественно истинно).

