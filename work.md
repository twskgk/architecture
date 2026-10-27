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
**Дано:** $l \perp a$, $l \perp b$, $a, b \subset \pi$, $l \not\perp c$, $c \subset \pi$.  
**Решение:**  
- Если $l \perp \pi$, то $l \perp \forall x \subset \pi$;  
- $l \not\perp c \Rightarrow l \not\perp \pi$;  
- $l \perp a$, $l \perp b$, $a, b \subset \pi$, $l \not\perp \pi \Rightarrow a \parallel b$.  
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

## Задача 5
**Дано:** $((\overline{X} \leftrightarrow \overline{Y}) \rightarrow (Y \wedge X)) \vee (X \rightarrow Y)$.  
**Решение:**  
- $\overline{X} \leftrightarrow \overline{Y} = X \leftrightarrow Y$;  
- $X \leftrightarrow Y = (X \wedge Y) \vee (\overline{X} \wedge \overline{Y})$;  
- $(X \leftrightarrow Y) \rightarrow (Y \wedge X) = \overline{(X \leftrightarrow Y)} \vee (Y \wedge X)$;  
- $\overline{(X \leftrightarrow Y)} = (X \wedge \overline{Y}) \vee (\overline{X} \wedge Y)$;  
- $\overline{(X \leftrightarrow Y)} \vee (Y \wedge X) = (X \wedge \overline{Y}) \vee (\overline{X} \wedge Y) \vee (X \wedge Y)$;  
- $X \rightarrow Y = \overline{X} \vee Y$;  
- Итоговое выражение: $((X \wedge \overline{Y}) \vee (\overline{X} \wedge Y) \vee (X \wedge Y)) \vee (\overline{X} \vee Y)$;  
- $\overline{X} \vee Y$ покрывает все возможные комбинации значений.  
**Ответ:** $1$.
