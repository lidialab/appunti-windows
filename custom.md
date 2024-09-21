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
