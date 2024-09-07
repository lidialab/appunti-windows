# File Batch
I file batch sono script che possono essere eseguiti da cmd.exe che ne è interprete e ambiente di runtime.

## Finestra cmd

```color 0F``` colore fore, colore back

```mode 84,42 ``` Qtà di colonne e righe con cui si apre la finestra della shell

```title titolo_della_finestra```

## Commenti
```rem ```

## Istruzione echo

```@echo off```

```echo testo con spazi```

```echo.``` lascia una riga vuota

```echo testo>"percorso_file"``` scrive (o sovrascrive)

```echo testo>>"percorso_file"``` accoda

```&``` per legare più istruzioni

## Etichette per i GOTO
```:nome_etichetta ```

## Variabili
Definire una variabile
```set nome_variabile=valore```

Usare una variabile
```%nome_variabile%```

## Comandi / istruzioni

```cls```

```explorer URL```

```goto nome_etichetta ```

```if exist "percorso_file" (fai qualcosa) else (fai altro) ```

```pause```

```pause >nul```

```start "nome_eseguibile"```

```type nomefile```

multi testo > file
```
(
echo testo1
echo testo2
)>"percorso_file"
```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```

``` ```
``` ```
``` ```
