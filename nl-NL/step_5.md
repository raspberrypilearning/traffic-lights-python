## Volgorde verkeerslichten

1. De `on` functie stelt je in staat een licht aan te schakelen. Je kunt `sleep` gebruiken om te pauzeren tussen opdrachten. Probeer dit voorbeeld eens om de lichten achter elkaar in te schakelen:
    
    ```python
from gpiozero import LED
from time import sleep

rood = LED (22)
oranje = LED (27)
groen = LED (17)

rood.on()
sleep(1)
oranje.on()
sleep(1)
groen.on()
sleep (1)
```

De belangrijkste bedieningselementen voor LED's zijn `on` aan, `off` uit, `toggle` wissel en `blink` knipperen.

2. Probeer de lichten achter elkaar in en uit te schakelen:
    
    ```python
rood.off()
groen.on()
sleep(1)
groen.off()
oranje.on()
sleep(1)
oranje.off()
rood.on()
sleep(1)
```

3. Probeer dit te herhalen door de code in een `while` lus te zetten:
    
    ```python
while True: red.on () slaap (1) amber.on () slaap (1) green.on () slaap (1) red.off () slaap (1) amber.off () slaap (1) groen. uit()
```

4. Nu weet je hoe je de lichten en de pauzes tussen opdrachten afzonderlijk kunt besturen, kun je nu een goede volgorde en tijdsduur voor een verkeerslicht maken? De volgorde is:

- Rood uit, groen aan
- Groen uit, oranje aan
- Oranje uit, rood aan
- Rood en oranje aan
- Groen aan

Het is belangrijk om na te denken over de tijdsduur van elk licht. Hoe lang moet het licht aan blijven in elke fase?

Nadat je het verkeerslicht hebt voltooid, kunt je proberen een knop en een zoemer toe te voegen om een ​​interactieve versie voor een zebrapad te maken.