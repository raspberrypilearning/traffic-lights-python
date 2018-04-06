## Vezéreld a LED-eket

1. Nyisd meg a Python 3-at a főmenüből, majd nyiss meg egy új fájlt.

2. Add meg a következő kódot:
    
    ```python
from gpiozero import LED piros = LED(22) piros.blink()
```

3. Mentsd el a programot és nyomd meg az **F5** -t hogy futtasd a kódodat. Most láthatod, hogy a piros lámpa fénye folyamatosan ki-be kapcsol.

4. Most változtass a kódodon és add hozzá a másik két lámpát a különböző villanási sebességekkel:
    
    ```python
from gpiozero import LED piros = LED(22) sárga = LED(27) zöld = LED(17) piros.blink(1, 1) sárga.blink(2, 2) zöld.blink(3, 3)
```

5. Futtasd újra a kódot, és látni fogod, hogy a három lámpa különböző sebességgel villog.

6. Ha egy nagyobb szám a lámpa villogását lassítja, akkor milyen szám gyorsítja a fényeket? Próbáld meg gyorsítani a fényeket.