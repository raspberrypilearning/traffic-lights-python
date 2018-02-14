## Steuere die LEDs

1. Öffne Python 3 aus dem Hauptmenü und öffne eine neue Datei.

2. Geben Sie den folgenden Code ein:
    
    ```python
from gpiozero import LED 

rot = LED (22) 

red.blink ()
```

3. Speichern Sie nun Ihr Programm und drücken Sie **F5** um deinen Code auszuführen. Sie sollten sehen, dass das rote Licht kontinuierlich blinkt.

4. Ändern Sie nun Ihren Code, um die anderen zwei Lichter einzuführen und sie mit verschiedenen Geschwindigkeiten blinken zu lassen:
    
    ```python
von gpiozero importieren LED rot = LED (22) gelb = LED (27) grün = LED (17) rot.blink (1, 1) amber.blink (2, 2) grün.blink (3, 3)
```

5. Führen Sie Ihren Code erneut aus und Sie sollten die drei Lichter mit unterschiedlichen Geschwindigkeiten blinken sehen.

6. Wenn eine größere Zahl ein Licht langsamer blinkt, welche Zahl würde es schneller laufen lassen? Versuche, deine Lichter schneller blinken zu lassen.