## Irányítsa a LED-eket

1. Nyissa meg a Python 3-at a főmenüből, és nyisson meg egy új fájlt.

2. Adja meg a következő kódot:
    
    ```python
a gpiozero importból LED piros = LED (22) red.blink ()
```

3. Most mentse el a programot, és nyomja meg a **F5** futtatni a kódot. A piros lámpát folyamatosan be kell kapcsolni és ki kell kapcsolni.

4. Most módosítsa a kódot, hogy bemutassa a másik két lámpát, és különböző sebességgel villogjon:
    
    ```python
a gpiozero import LED piros = LED (22) borostyánsárga = LED (27) zöld = LED (17) red.blink (1, 1) amber.blink (2, 2) green.blink (3, 3)
```

5. Futtassa újra a kódot, és látni fogja, hogy a három lámpa villog, különböző sebességgel.

6. Ha egy nagyobb szám a lámpa villogását lassítja, akkor mekkora lesz a gyorsabb futás? Próbálja meg villogni a fények gyorsabban.