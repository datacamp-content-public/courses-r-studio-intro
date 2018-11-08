---
title: RStudio
description: 'Allgemeine Fragen zu RStudio'
---

## Anwendungsbereich R-Studio

```yaml
type: PureMultipleChoiceExercise
key: 85cda17d46
xp: 50
```

In welchen der folgend genannten Fälle ist RStudio eine ideale Anwendung?

`@hint`
Vielleicht solltest du ganz kurz mal die Homepage von R-Studio ansehen

`@possible_answers`
- [Um R-Programme zu schreiben, den Programmablauf zu testen und Projektbasiert zu arbeiten.]
- Um die Ausgabe von R-Programmen tabellarisch und graphisch dazustellen.
- Um Graphiken und Tabellen von R-Programmen APA-konform darzustellen.
- Um R-Programme in lauffähige .exe Dateien umzuwandeln.

`@feedback`
- Nicht schlecht für den Anfang!
- Nein, dafür kann es verwendet werden, aber es ist nicht die ideale Anwendung.
- Kann man machen, aber dafür ist R-Studio nicht gedacht.
- R ist eine Interpreter-Sprache, die Programm müssen daher nicht kompiliert werden.

---

## Konsolenfenster

```yaml
type: PureMultipleChoiceExercise
key: 80a18784d0
xp: 50
```

Für was wird in R-Studio das Konsolenfenster verwendet?

`@hint`
Sieh mal im Web nach

`@possible_answers`
- [Um direkte R-Befehle abzusenden.]
- Um die R-Dateien zu verwalten.
- Um den Ablauf von R-Programmen zu kontrollieren.
- Um R-Programme zu schreiben und diese in einem Programmfile abzuspeichern.

`@feedback`
- Super!
- Das kann man besser im Dateimanager machen
- Dazu verwendet man den Debugger
- Dazu verwendet man das "Source-Fenster"

---

## Insert exercise title here

```yaml
type: NormalExercise
key: 1d6545be34
xp: 100
```

Bei dieser Aufgabe geht es darum, die Konsole von R-Studio als einfachen Taschenrechner zu verwenden.

`@instructions`
Berechnen Sie die Addition der Zahlen 2+28

`@hint`
Ergebnis sollte 30 sein, wenn du was anderes heraus bekommst dann passt was nicht

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
2+28
```

`@sct`
```{r}
ex() %>% check_code(c("2+28", "28+2"), fixed = TRUE)
```
