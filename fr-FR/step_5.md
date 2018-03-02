## Séquence de feux de signalisation

1. La fonction `on` vous permet d'allumer une lumière. Vous pouvez utiliser `sleep` pour faire une pause entre les commandes. Essayez cet exemple pour allumer les lumières en séquence:
    
    ```python
    from gpiozero import LED
    from time import sleep

    rouge = LED(22)
    ambre = LED(27)
    vert = LED(17)

    rouge.on()
    sleep(1)
    ambre.on()
    sleep(1)
    vert.on()
    sleep(1)
    ```

    Les commandes principales des LEDs sont les suivantes: `on`, `off`, `toggle` et `blink`.

2. Essayez d'allumer et d'éteindre les lumières dans l'ordre:
    
    ```python
    rouge.on()
    sleep(1)
    ambre.on()
    sleep(1)
    vert.on()
    sleep(1)
    rouge.off()
    sleep(1)
    ambre.off()
    sleep(1)
    vert.off()
    ```

3. Essayez de répéter ceci en plaçant le code dans une boucle `while` :
    
    ```python
    while True:
       rouge.on()
       sleep(1)
       ambre.on()
       sleep(1)
       vert.on()
       sleep(1)
       rouge.off()
       sleep(1)
       ambre.off()
       sleep(1)
       vert.off()
    ```

4. Maintenant que vous savez comment contrôler les lumières individuellement, et régler les pauses entre les commandes, pouvez-vous créer une séquence de feux de signalisation? La séquence suit:

- Vert allumé
- Ambre allumé
- Rouge allumé
- Rouge et ambre allumés
- Vert allumé

Il est important de penser au timing. Combien de temps les lumières doivent-elles rester allumées à chaque étape?

Une fois que vous avez terminé la séquence des feux de signalisation, vous pouvez essayer d'ajouter un bouton et un buzzer pour créer une version interactive.
