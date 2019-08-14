## Bedien de LED's

--- task ---

Open **Mu** vanuit het hoofdmenu.

---/task---

--- task ---

Voer de volgende code in:

```python
from gpiozero import 
LED 

rood = LED (22)

rood.blink ()
```

--- /task ---

--- task ---

Sla nu je programma op en druk op **F5** om je code uit te voeren. Het rode lampje zou continu aan en uit moeten gaan.

--- /task ---

--- task ---

Pas nu je code aan om de andere twee lichtjes te besturen en laat ze op verschillende snelheden knipperen:

```python
from gpiozero import LED
rood = LED (22)
oranje = LED (27)
groen = LED (17)

rood.blink(1, 1)
oranje.blink(2, 2)
groen.blink (3, 3)
```

-- /task ---

--- task ---

Voer je code opnieuw uit en je zou de drie lichtjes met verschillende snelheden moeten zien knipperen.

--- /task ---

--- task ---

Als een groter getal het lampje langzamer laat knipperen, welk getal zou het dan sneller laten knipperen? Probeer je LED's sneller te laten knipperen.

--- /task ---