## Volgorde verkeerslichten

1. De `on` functie stelt u in staat een licht aan te doen. U kunt `sleep` gebruiken om te pauzeren tussen opdrachten. Probeer dit voorbeeld om de lichten achter elkaar in te schakelen:
    
    ```python
van gpiozero import LED van tijdimport slaap rood = LED (22) oranje = LED (27) groen = LED (17) red.on () slaap (1) amber.on () slaap (1) green.on () slaap (1)
```

De belangrijkste bedieningselementen voor LED's zijn `on`, `uit`, `toggle` en `knipperen`.

2. Probeer de lichten achter elkaar in en uit te schakelen:
    
    ```python
red.on () slaap (1) amber.on () slaap (1) green.on () slaap (1) red.off () slaap (1) amber.off () slaap (1) green.off ()
```

3. Probeer dit te herhalen door de code in een `while` lus:
    
    ```python
while True: red.on () slaap (1) amber.on () slaap (1) green.on () slaap (1) red.off () slaap (1) amber.off () slaap (1) groen. uit()
```

4. Nu weet u hoe u de lichten afzonderlijk bedient en de pauzes tussen opdrachten kunt u een opeenvolging van verkeerslichten maken? De volgorde gaat:

- Groen aan
- Amber aan
- Rood aan
- Rood en oranje op
- Groen aan

Het is belangrijk om na te denken over timing. Hoe lang moet het licht aan blijven in elke fase?

Nadat u de reeks verkeerslichten hebt voltooid, kunt u proberen een knop en een zoemer toe te voegen om een ​​interactieve versie te maken.