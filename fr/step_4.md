## Contrôler les LED

1. Ouvrez Python 3 à partir du menu principal et ouvrez un nouveau fichier.

2. Entrez le code suivant:
    
    ```python
à partir de gpiozero import LED rouge = LED (22) red.blink ()
```

3. Maintenant, sauvegardez votre programme et appuyez sur **F5** pour exécuter votre code. Vous devriez voir la lumière rouge clignoter continuellement.

4. Maintenant, modifiez votre code pour introduire les deux autres lumières et faites-les clignoter à différentes vitesses:
    
    ```python
à partir de gpiozero LED d'importation rouge = LED (22) ambre = LED (27) vert = LED (17) red.blink (1, 1) amber.blink (2, 2) green.blink (3, 3)
```

5. Exécutez votre code à nouveau et vous devriez voir les trois lumières clignotant à des taux différents.

6. Si un plus grand nombre clignote plus lentement, quel nombre le ferait fonctionner plus vite? Essayez de faire clignoter vos lumières plus rapidement.