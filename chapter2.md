---
title: 'R Konsole'
description: ""
---

## Pfeiltasten

```yaml
type: PureMultipleChoiceExercise
key: 4131d96f57
xp: 50
```

Welche Auswirkung haben die Pfeiltasten (nach oben, nach unten) in der Konsole?

`@hint`


`@possible_answers`
- Bewegen den Cursor in ein anderes Fenster von RStudio.
- Bewirken nichts spezielles.
- [Blättern durch die bereits eingegebenen Befehle (Historie)]

`@feedback`
- Nein, tun sie nicht.
- Bewirken schon etwas, denk mal nach oder probiers einfach mal aus!
- Ja, die Historie der bereits eingegeben Befehle wird damit durchblättert.

---

## Terminalfenster

```yaml
type: PureMultipleChoiceExercise
key: a756ca66a6
xp: 50
```

Das Terminalfenster in der Konsole ermöglicht:

`@hint`


`@possible_answers`
- R zu beenden
- [fortgeschrittenen Programmkontrolle zu starten]
- R Code in externe Anwendungen zu kopiern

`@feedback`
- Falsch
- Richtig
- Falsch

---

## Polyomberechnung

```yaml
type: NormalExercise
key: 62baa23c55
xp: 100
```

Berechne das Ergebnis für das folgende Polynom 3 mal **Var1** plus 2.8 mal **Var1** zum Quadrat plus 10 mal die Wurzel von **Var1**.

`@instructions`
Da für x bereits Werte geladen sind, brauchst du bezüglich der Variablenerstellung nichts mehr machen!

`@hint`


`@pre_exercise_code`
```{r}
Var1 <- c(2, 4 ,8)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
3*Var1+2.8*Var1^2+10*sqrt(Var1)
```

`@sct`
```{r}
ex() %>% check_code(c("3*Var1+2.8*Var1^2+10*sqrt(Var1)"), fixed = TRUE)
```

---

## Mehrfachvergleiche

```yaml
type: NormalExercise
key: 3890de6534
xp: 100
```

Prüfe in einer Codezeile, ob 3 * 4 gleich 2 * 6 UND 5 * 12 gleich 60 ist.

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
3*4 == 2*6 & 5*12 == 60
```

`@sct`
```{r}
ex() %>% check_code(c("3*4 == 2*6 & 5*12 == 60"), fixed = TRUE)
```

---

## Variablenberechnung

```yaml
type: TabExercise
key: ac4cf56bea
xp: 100
```

Weise der Variablen **Var1** den Wert **5** zu

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: df8e973c46
xp: 50
```

`@instructions`
Berechne nun die 3te Potenz der Variablen Var1

`@hint`


`@sample_code`
```{r}

```

`@solution`
```{r}
Var1 <- 5
Var1^3
```

`@sct`
```{r}
ex() %>% check_code(c("Var1 <- 5", "Var1^3"), fixed = TRUE)
```

***

```yaml
type: MultipleChoiceExercise
key: 4f4dfefa9f
xp: 50
```

`@question`
Das Ergebnis lautet?

`@possible_answers`
- 100
- [125]
- 150

`@hint`


`@sct`
```{r}
125
```

---

## Variablen und einfache Funktionen

```yaml
type: TabExercise
key: fd86f277a3
xp: 100
```

In dieser Übung verwenden wir Variablen und einfache Funktionen. Bei diesem Beispiel geht es um die z-Transformation einer Zahl **x** aus der Menge einer Stichprobe **SP**. Die Stichprobe wurde aus einer normalverteilten Grundgesamtheit gezogen und hat einen Umfang von N = 300, einen Mittelwert von MW = 100 und eine Streuung von SD = 15. Die Variable SP steht bereits zur weiteren Verwendung zur Verfügung!

`@pre_exercise_code`
```{r}
SP <-  rnorm(300, mean = 100, sd = 15)
```

***

```yaml
type: NormalExercise
key: 69438ace6d
xp: 100
```

`@instructions`
Die z-Transformation eines Elementes **x** aus der Stichprobe berechnet sich aus der Differenz von x zum MW der Stichprobe, geteilt durch die Standardabweichung SD. Berechne die z-Transformation für x = 90 und speichere das Ergebnis in der Variablen **x90** und gib den Wert der Variablen **x90** in der Konsole aus!

`@hint`
Weise im ersten Schritt der Variablen x den Wert 90 zu. Im nächsten Schritt verwende die Funktionen mean() und sd() um die Formel zur Berechnung der z-Transformation zu erstellen.

`@sample_code`
```{r}

```

`@solution`
```{r}
x <- 90
x90 <- (x - mean(SP)) / sd(SP)
x90
```

`@sct`
```{r}
ex() %>% check_code(c("x<-90", "x90 <- (x - mean(SP)) / sd(SP)", "x90"), fixed = TRUE)
```
