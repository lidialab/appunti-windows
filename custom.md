# Personalizzazioni Windows

## Windows 11

### Menu contestuale avanzato

Combinazione di tasti: ```MAIUSC + F10```

Registro Windows:
- Nella sezione ```HKCU\SOFTWARE\CLASSES\CLSID\```
- creare la chiave ```{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}```
- al suo interno creare la chiave ```InprocServer32```
- con nessun valore impostato
- riavviare explorer

Per aggiungere la voce di registro da terminale:
```reg add "HKCU\SOFTWARE\CLASSES\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /ve /f```

```/ve``` --> aggiunge un nome valore vuoto per la chiave

```/f``` --> sovrascrive senza chiedere conferma

Riavviare explorer da terminale:
- ```taskkill /im explorer.exe /f```
 
```/im``` --> nome immagine da killare

```/f``` --> forzato

- ```explorer.exe```

## Layout di tastiera personalizzata

Installa ```.NET Framework 3.5``` (che include anche .NET 2.0 e 3.0) da ```Pannello di controllo > Programmi > Programmi e funzionalità > Attivazione o disattivazione delle funzionalità Windows```

Installa ```Microsoft Keyboard Layout Creator``` (MSKLC)[https://www.microsoft.com/en-us/download/details.aspx?id=102134]

Crea il tuo layout, crea il pacchetto, installalo
