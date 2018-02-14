## Controlla i LED

1. Apri Python 3 dal menu principale e apri un nuovo file.

2. Inserisci il seguente codice:
    
    ```python
da gpiozero import LED rosso = LED (22) red.blink ()
```

3. Ora salva il tuo programma e premi **F5** per eseguire il tuo codice. Dovresti vedere la luce rossa accendere e spegnere continuamente.

4. Ora modifica il tuo codice per introdurre le altre due luci e farle lampeggiare a velocità diverse:
    
    ```python
da gpiozero import LED rosso = LED (22) ambra = LED (27) verde = LED (17) rosso.blink (1, 1) ambra.blink (2, 2) green.blink (3, 3)
```

5. Esegui nuovamente il codice e dovresti vedere le tre luci lampeggiare a velocità diverse.

6. Se un numero maggiore fa rallentare leggermente la luce, quale numero lo renderebbe più veloce? Prova a far lampeggiare più velocemente le tue luci.