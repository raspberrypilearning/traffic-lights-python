## Steuere die LEDs

1. Öffne Python 3 aus dem Hauptmenü und öffne eine neue Datei.

2. Gib den folgenden Code ein:
    
    ```python
from gpiozero import LED 

rot = LED (22) 

rot.blink ()
```

3. Speichere nun dein Programm und drücke **F5** um deinen Code auszuführen. Du solltest sehen, dass das rote Licht kontinuierlich blinkt.

4. Ändere nun deinen Code, um die anderen zwei Lichter anzusteuern und sie mit verschiedenen Geschwindigkeiten blinken zu lassen:
    
    ```python
from gpiozero import LED

rot = LED(22)
bernstein = LED(27)
gruen = LED(17)

rot.blink(1, 1)
bernstein.blink(2, 2)
gruen.blink(3, 3)
```

5. Führe deinen Code erneut aus und du sollten die drei Lichter mit unterschiedlichen Geschwindigkeiten blinken sehen.

6. Wenn eine größere Zahl ein Licht langsamer blinken läßt, welche Zahl würde es schneller laufen lassen? Versuche, deine Lichter schneller blinken zu lassen.