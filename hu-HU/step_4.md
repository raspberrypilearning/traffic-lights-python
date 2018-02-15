## Irányítsd a LED-eket

1. A főmenüből nyisd meg a Python 3-at, majd nyiss meg egy új fájlt.

2. Add meg a következő kódot:
    
    ```python
a gpiozero importból LED piros = LED (22) red.blink ()
```

3. Mentsd el a programot és nyomd meg a **F5** -t, hogy futtasd a kódot. Most láthatod, hogy a piros lámpa fénye folyamatosan ki-be kapcsol.

4. Most változtass a kódodon es add hozzá a másik két lámpát a kulonbozo villanasi sebesseggekkel:
    
    ```python
a gpiozero import LED piros = LED (22) borostyánsárga = LED (27) zöld = LED (17) red.blink (1, 1) amber.blink (2, 2) green.blink (3, 3)
```

5. Futtassa újra a kódot, és látni fogja, hogy a három lámpa villog, különböző sebességgel.

6. Ha egy nagyobb szám a lámpa villogását lassítja, akkor mekkora lesz a gyorsabb futás? Próbálja meg villogni a fények gyorsabban.