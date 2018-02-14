## Verkehrsampel Sequenz

1. Die `on` Funktion ermöglicht es, ein Licht einzuschalten. Du kannst `sleep` verwenden um zwischen Befehlen anzuhalten. Probieren Sie dieses Beispiel aus, um die Lichter nacheinander einzuschalten:
    
    ```python
from gpiozero import LED
from time import sleep

red = LED(22)
amber = LED(27)
green = LED(17)

red.on()
sleep(1)
amber.on()
sleep(1)
green.on()
sleep(1)
```

Die Hauptbefehle für LEDs sind `on`, `off`, `toggle` und `blink` (ein-, aus- und umschalten, blinken).

2. Versuchen Sie, die Lichter der Reihe nach ein- und auszuschalten:
    
    ```python
red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green.off ()
```

3. Versuche dies zu wiederholen, indem du den Code in eine `while` Schleife einfügst:
    
    ```python
während True: red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green. aus()
```

4. Jetzt weist du, wie man die Lichter individuell steuert und die Pausen zwischen den Befehlen einstellt. Kannst du eine Ampelsequenz erstellen? Die Reihenfolge lautet:

- Grün an
- Bernstein an
- Rot an
- Rot und Bernstein an
- Grün an

Es ist wichtig, über das Timing nachzudenken. Wie lange sollten die Lichter in jeder Phase eingeschaltet bleiben?

Sobald du die Ampelsequenz abgeschlossen hast, kannst du versuchen, einen Taster und einen Summer hinzuzufügen, um eine interaktive Version zu erstellen.