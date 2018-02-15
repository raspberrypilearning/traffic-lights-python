## Controlla i LED

1. Apri Python 3 dal menu principale e apri un nuovo file.

2. Inserisci il seguente codice:
    
    ```python
from gpiozero import LED 

rosso = LED(22) 

rosso.blink()
```

3. Ora salva il programma e premi **F5** per eseguire il codice. Dovresti vedere la luce rossa accendersi e spegnersi continuamente.

4. Ora modifica il codice per introdurre le altre due luci e farle lampeggiare a velocità diverse:
    
    ```python
from gpiozero import LED

rosso = LED(22) 
ambra = LED(27)
verde = LED(17) 

rosso.blink(1, 1) 
ambra.blink(2, 2) 
verde.blink(3, 3)
```

5. Eseguendo nuovamente il codice dovresti vedere le tre luci lampeggiare a velocità differenti.

6. Se un numero più alto fa rallentare leggermente la velocità a cui lampeggia la luce, con quale numero andrebbe più veloce? Prova a far lampeggiare più velocemente i LED.