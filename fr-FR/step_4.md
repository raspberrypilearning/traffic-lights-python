## Contrôlez les LEDs

1. Ouvrez Python 3 du menu principal et ouvrez un nouveau fichier.

2. Entrez le code suivant:
    
    ```python
from gpiozero import LED

rouge = LED(22)

rouge.blink()
```

3. Maintenant, sauvegardez votre programme et appuyez sur **F5** pour faire fonctionner votre code. Vous devriez voir la lumière rouge clignote continuellement.

4. Maintenant, modifiez votre code pour introduire les deux autres lumières et faites-les clignoter à différentes vitesses:
    
    ```python
from gpiozero import LED

rouge = LED(22)
ambre = LED(27)
vert = LED(17)

rouge.blink(1, 1)
ambre.blink(2, 2)
vert.blink(3, 3)
```

5. Faites fonctionner votre code à nouveau et vous devriez voir les trois lumières clignotent aux taux différents.

6. Si un plus grand nombre fait clignoter une lumière plus lentement, quel nombre le ferait fonctionner plus vite? Essayez de faire clignoter vos lumières plus rapidement.