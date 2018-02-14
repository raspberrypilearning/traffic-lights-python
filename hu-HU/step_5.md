## A közlekedési lámpa sorrendje

1. A `on` funkció lehetővé teszi, hogy bekapcsoljon egy világítást. Használhatja a `sleep` -t szüneteltetni a parancsok között. Próbálja meg ezt a példát a lámpák sorrendben történő bekapcsolásához:
    
    ```python
a gpiozero import LED az idő import alvásakor piros = LED (22) borostyánsárga = LED (27) zöld = LED (17) red.on () alvás (1) amber.on () sleep (1) green.on (1)
```

A LED-ek fő vezérlése: `on`, `off`, `váltás` és 123_6_6_321 | villog</code>.

2. Próbálja meg világítani és kikapcsolni a lámpákat:
    
    ```python
() sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green.off
```

3. Próbálja meg ezt ismételni úgy, hogy a kódot a `, míg` hurok:
    
    ```python
míg a True: red.on () alvás (1) amber.on () sleep (1) green.on () sleep (1) red.off () alvás (1) amber.off () alvás (1) zöld. ki()
```

4. Most már tudod, hogyan kell egyedileg irányítani a fényeket, és a parancsok közötti szünetek idejét, létrehozhatsz egy közlekedési lámpa sorozatát? A szekvencia megy:

- Zölden
- Borostyán
- Piros
- Piros és sárga
- Zölden

Fontos időzni. Mennyi ideig kell a fények maradni minden szakaszban?

Miután befejezte a közlekedési lámpák sorozatát, érdemes megpróbálnia hozzáadni egy gombot és egy zümmögőt, hogy interaktív verziót készítsen.