## Séquence de feux de signalisation

1. Le `on` fonction vous permet d'allumer une lumière. Vous pouvez utiliser `sleep` pour faire une pause entre les commandes. Essayez cet exemple pour allumer les lumières en séquence:
    
    ```python
à partir de gpiozero import LED à partir de l'heure d'importation sommeil rouge = LED (22) ambre = LED (27) vert = LED (17) red.on () sommeil (1) amber.on () sommeil (1) green.on () sommeil (1)
```

Les commandes principales des voyants sont les suivantes: `on`, `off`, `toggle` et `blink`.

2. Essayez d'allumer et d'éteindre les lumières dans l'ordre:
    
    ```python
red.on () sleep (1) amber.on () sleep (1) vert.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green.off ()
```

3. Essayez de répéter ceci en plaçant le code dans un `while` boucle:
    
    ```python
while Vrai: red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) vert. de()
```

4. Maintenant, vous savez comment contrôler les lumières individuellement, et le temps des pauses entre les commandes, pouvez-vous créer une séquence de feux de circulation? La séquence va:

- Vert sur
- Ambre sur
- Rouge sur
- Rouge et ambre sur
- Vert sur

Il est important de penser au timing. Combien de temps les lumières doivent-elles rester allumées à chaque étape?

Une fois que vous avez terminé la séquence des feux de circulation, vous pouvez essayer d'ajouter un bouton et un buzzer pour créer une version interactive.