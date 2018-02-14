## Verkehrsampel Sequenz

1. Die `on` Funktion ermöglicht es, ein Licht einzuschalten. Du kannst `sleep` verwenden um zwischen Befehlen anzuhalten. Probiere dieses Beispiel aus, um die Lichter nacheinander einzuschalten:
    
    ```python
from gpiozero import LED
from time import sleep

rot = LED(22)
bernstein = LED(27)
gruen = LED(17)

rot.on()
sleep(1)
bernstein.on()
sleep(1)
gruen.on()
sleep(1)
```

Die Hauptbefehle für LEDs sind `on`, `off`, `toggle` und `blink` (ein-, aus- und umschalten, blinken).

2. Versuche die Lichter der Reihe nach ein- und auszuschalten:
    
    ```python
rot.on()
sleep(1)
bernstein.on()
sleep(1)
gruen.on()
sleep(1)
rot.off()
sleep(1)
bernstein.off()
sleep(1)
gruen.off()
```

3. Versuche dies zu wiederholen, indem du den Code in eine `while` Schleife einfügst:
    
    ```python
while True:
   rot.on()
   sleep(1)
   bernstein.on()
   sleep(1)
   gruen.on()
   sleep(1)
   rot.off()
   sleep(1)
   bernstein.off()
   sleep(1)
   gruen.off()
```

4. Jetzt weist du, wie man die Lichter individuell steuert und die Pausen zwischen den Befehlen einstellt. Kannst du eine Ampelsequenz erstellen? Die Reihenfolge lautet:

- Grün an
- Bernstein an
- Rot an
- Rot und Bernstein an
- Grün an

Es ist wichtig, über das Timing nachzudenken. Wie lange sollten die Lichter in jeder Phase eingeschaltet bleiben?

Sobald du die Ampelsequenz abgeschlossen hast, kannst du versuchen, einen Taster und einen Summer hinzuzufügen, um eine interaktive Version zu erstellen.