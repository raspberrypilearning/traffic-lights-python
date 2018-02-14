## Steuere die LEDs

1. Öffne Python 3 aus dem Hauptmenü und öffne eine neue Datei.

2. Geben Sie den folgenden Code ein:
    
    ```python
from gpiozero import LED 

rot = LED (22) 

red.blink ()
```

3. Speicher nun dein Programm und drücke **F5** um deinen Code auszuführen. Sie sollten sehen, dass das rote Licht kontinuierlich blinkt.

4. Ändern Sie nun Ihren Code, um die anderen zwei Lichter anzusteuern und sie mit verschiedenen Geschwindigkeiten blinken zu lassen:
    
    ```python
from gpiozero import LED

red = LED(22)
amber = LED(27)
green = LED(17)

red.blink(1, 1)
amber.blink(2, 2)
green.blink(3, 3)
```

5. Führe deinen Code erneut aus und du sollten die drei Lichter mit unterschiedlichen Geschwindigkeiten blinken sehen.

6. Wenn eine größere Zahl ein Licht langsamer blinken läßt, welche Zahl würde es schneller laufen lassen? Versuche, deine Lichter schneller blinken zu lassen.