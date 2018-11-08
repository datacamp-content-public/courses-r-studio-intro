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

## Ctrl-L

```yaml
type: PureMultipleChoiceExercise
key: 5fbf47b162
xp: 50
```

Was bewirkt der Ctrl-L im Konsolenfenster?

`@hint`
L wie Leer

`@possible_answers`
- Listet die letzt verwendeten Befehle auf
- [Löscht den Inhalt des Konsolenfenster]
- Laden von Dateien
- Löschen der Variablen im Environment

`@feedback`
Sehr gut, nnur weiter so!

---

## Pfeiltasten

```yaml
type: PureMultipleChoiceExercise
key: 6fe296d94b
xp: 50
```

Was bewirken die Pfeiltasten (Up/Down) im Konsolenfenster?

`@hint`
Erspart eventuell Tipparbeit.

`@possible_answers`
- Vergrößert das Konsolenfenster
- Verkleinert das Konsolenfenster
- [Zeigt die Historie der bereits verwendeten Befehle]
- Hat keine Wirkung

`@feedback`
Na also, passt ja alles.

---

## Tab

```yaml
type: PureMultipleChoiceExercise
key: 0b6e4acaf0
xp: 50
```

Der Tabulator hat im Konsolenfenster eine besondere Eigenschaft. Welche der nachfolgenden

`@hint`
Ergänzung von Befehlen

`@possible_answers`
- Fügt einen fest vorgegebenen Abstand an Leerzeichen ein.
- [Sucht nach einer Funktion, die mit denselben Buchstaben beginnen wie bereits eingegeben und zeigt diese Funktionen einerseits an, und vervollständigt den Namen des begonnen Funktionsnamen]
-  Wechselt vom Konsolefenster zum Environmentfenster.
-  Wechselt vom Konsolefenster zum Filefenster.

`@feedback`


---

## Tab-completion

```yaml
type: MultipleChoiceExercise
key: 710bb8bb0e
xp: 50
```

Berechne den Mittelwert des Vektors **v1** (der Vektor wurde bereits in den Arbeitsspeicher geladen und ist mit eben diesen Namen verfügbar). Wenn du in der Konsole v1 und Eingabe eingibst, siehst du die Werte die in diesem Vektor gespeichtert sind.

Verwende die Tab-completion von RStudio sowohl beim Funktionsnamen wie auch innerhalb der Funktion.

`@possible_answers`
- 5.4
- [7.6]
- 10.45
- 12.23

`@hint`
Verwende die Funktion mean() und die Tab-completion Funktion von R-Studio

`@pre_exercise_code`
```{r}
v1 <- c(3, 12, 13, 4, 6)
```

`@sct`
```{r}
ex() %>% check_function("mean") %>% check_result() %>% check_equal()
```

---

## Console als Rechner

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
