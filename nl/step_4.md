## Bedien de LED's

1. Open Python 3 in het hoofdmenu en open een nieuw bestand.

2. Voer de volgende code in:
    
    ```python
van gpiozero importeren LED rood = LED (22) red.blink ()
```

3. Sla nu je programma op en druk op **F5** om uw code uit te voeren. Je zou het rode lampje continu aan en uit moeten zien flitsen.

4. Pas nu uw code aan om de andere twee lampen te introduceren en laat ze op verschillende snelheden knipperen:
    
    ```python
van gpiozero importeren LED rood = LED (22) oranje = LED (27) groen = LED (17) rood. knipperen (1, 1) amber.blink (2, 2) green.blink (3, 3)
```

5. Voer uw code opnieuw uit en u zou de drie lampjes met verschillende snelheden moeten zien knipperen.

6. Als een groter getal het lampje langzamer laat knipperen, welk cijfer zou het dan sneller laten werken? Probeer je lichten sneller te laten knipperen.