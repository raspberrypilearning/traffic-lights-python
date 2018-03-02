## Séquence de feux de signalisation

1. La fonction `on` vous permet d'allumer un feux. Vous pouvez utiliser `sleep` pour faire une pause entre les commandes. Essayez cet exemple pour allumer les feux en séquence:
    
    ```python
    from gpiozero import LED
    from time import sleep

    rouge = LED(22)
    jaune = LED(27)
    vert = LED(17)

    rouge.on()
    sleep(1)
    jaune.on()
    sleep(1)
    vert.on()
    sleep(1)
    ```

Les commandes principales pour les DELs sont `on`, `off`, `toggle` et `blink`.

2. Essayez d'allumer et d'éteindre les feux en séquence:
    
    ```python
    rouge.on()
    sleep(1)
    jaune.on()
    sleep(1)
    vert.on()
    sleep(1)
    rouge.off()
    sleep(1)
    jaune.off()
    sleep(1)
    vert.off()
    ```

3. Essayez de répéter ceci en plaçant le code dans une boucle `while`:
    
    ```python
    while True:
       rouge.on()
       sleep(1)
       jaune.on()
       sleep(1)
       vert.on()
       sleep(1)
       rouge.off()
       sleep(1)
       jaune.off()
       sleep(1)
       vert.off()
    ```

4. Maintenant vous savez comment contrôler les feux individuellement et ajuster les poses entre les commandes. Pouvez-vous créer une séquence de feux de circulation? Voici la séquence:

- Vert allumé
- Jaune on
- Rouge on
- Rouge et ambre allumés
- Vert allumé

Il est important de penser à la durée de chacun des feux. Combien de temps chaque feux devrait-il rester allumé?

Une fois que vous aurez complété la séquence de feux de circulation, vous pourriez essayer d'y ajouter un bouton ou un avertisseur sonore pour la rendre interactive.
