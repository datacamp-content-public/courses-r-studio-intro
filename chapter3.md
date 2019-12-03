---
title: Homework
description: 'erste Hausübung'
---

## Vektoren erzeugen

```yaml
type: NormalExercise
key: f6db413b93
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Erzeugen Sie einen Vektor x, der aus den natürlichen Zahlen von 1 bis 10 besteht
  Hinweis: c(1,2,3,4,5,6,7,8,9,10) gilt nicht, es gibt eine einfachere Lösung!

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- c(x:y)

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
x <- c(1:10)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## Rechnen mit Vektoren

```yaml
type: NormalExercise
key: fb8781ebba
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
(a) Berechnen Sie die Summe von x und weisen Sie das Ergebnis einem Vektor y zu.

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- sum()

`@pre_exercise_code`
```{r}
x <- c(1:10)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
y <- sum(x)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## Vektoren verknüpfen

```yaml
type: NormalExercise
key: b2adec3b85
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
(b) Erzeugen Sie einen neuen Vektor z der x und danach y enthält.

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- c()
- This is an example hint.

`@pre_exercise_code`
```{r}
x <- c(1:10)
y <- sum(x)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
z <- c(x,y)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```
