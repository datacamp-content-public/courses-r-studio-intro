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

Berechne das Ergebnis für das folgende Polynom 3 mal x plus 2.8 mal x zum Quadrat plus 10 mal die Wurzel von x.

`@instructions`
Da für x bereits Werte geladen sind, brauchst du bezüglich der Variablenerstellung nichts mehr machen!

`@hint`


`@pre_exercise_code`
```{r}
x <- c(2, 4 ,8)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
3*x+2.8*x^2+sqrt(x)
```

`@sct`
```{r}
ex() %>% check_code(c("3*x+2.8*x^2+sqrt(x)"), fixed = TRUE)
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
A <- 5
```

***

```yaml
type: NormalExercise
key: df8e973c46
xp: 50
```

`@instructions`
Berechne nun die 3te Potenz der Variablen A

`@hint`


`@sample_code`
```{r}

```

`@solution`
```{r}
A <- 5
A^3
```

`@sct`
```{r}
ex() %>% check_code(c("A<-5", "A^3"), fixed = TRUE)
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
- 125
- 150

`@hint`


`@sct`
```{r}
- falsch
- richtig
- falsch
```
