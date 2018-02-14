## Verkehrsampel Sequenz

1. Die `on` Funktion ermöglicht es, ein Licht einzuschalten. Sie können `sleep` verwenden zwischen Befehlen anhalten. Probieren Sie dieses Beispiel aus, um die Lichter nacheinander einzuschalten:
    
    ```python
von gpiozero import LED von time import sleep rot = LED (22) amber = LED (27) grün = LED (17) rot.ein () sleep (1) amber.on () sleep (1) green.on () sleep (1)
```

Die Hauptsteuerungen für LEDs sind `on`, `off`, `toggle` und `blink`.

2. Versuchen Sie, die Lichter der Reihe nach ein- und auszuschalten:
    
    ```python
red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green.off ()
```

3. Versuchen Sie dies zu wiederholen, indem Sie den Code in ein `while` einfügen Schleife:
    
    ```python
während True: red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green. aus()
```

4. Jetzt wissen Sie, wie man die Lichter individuell steuert und die Pausen zwischen den Befehlen einstellt. Können Sie eine Ampelsequenz erstellen? Die Reihenfolge lautet:

- Grün an
- Bernstein an
- Rot an
- Rot und Bernstein an
- Grün an

Es ist wichtig, über das Timing nachzudenken. Wie lange sollten die Lichter in jeder Phase eingeschaltet bleiben?

Sobald Sie die Ampelsequenz abgeschlossen haben, können Sie versuchen, eine Schaltfläche und einen Summer hinzuzufügen, um eine interaktive Version zu erstellen.