## Contrôlez les DELs

\---tâche\---

Open **Mu** from the main menu.

\---tâche\---

\---tâche\---

Entrez le code suivant:

```python
from gpiozero import LED

rouge = LED(22)

rouge.blink()
```

\---tâche\---

\---tâche\---

Maintenant, sauvegardez votre programme et appuyez sur **F5** pour faire exécuter votre code. Vous devriez voir le feux rouge clignoter continuellement.

\---tâche\---

\---tâche\---

Maintenant modifiez votre code pour y ajouter les deux autres feux et faites les clignoter à différentes vitesses:

```python
from gpiozero import LED

rouge = LED(22)
jaune = LED(27)
vert = LED(17)

rouge.blink(1, 1)
jaune.blink(2, 2)
vert.blink(3, 3)
```

\---tâche\---

\---tâche\---

Exécutez votre code à nouveau et vous devriez voir les trois feux clignoter à des vitesses différentes.

\---tâche\---

\---tâche\---

Si un nombre plus élevé fait clignoter un feux plus lentement, quel nombre le ferait clignoter plus rapidement? Essayez de faire clignoter vos feux plus rapidement.

\---tâche\---