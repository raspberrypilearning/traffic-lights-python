## Sequenza dei semafori

1. Il `on` la funzione ti permette di accendere una luce. È possibile utilizzare `sleep` per mettere in pausa tra i comandi. Prova questo esempio per accendere le luci in sequenza:
    
    ```python
da gpiozero import LED dall'ora importazione sleep rosso = LED (22) ambra = LED (27) verde = LED (17) red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1)
```

I controlli principali per i LED sono `on`, `off`, `toggle` e `lampeggia`.

2. Prova ad accendere e spegnere le luci in sequenza:
    
    ```python
red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) green.off ()
```

3. Prova a ripetere questo inserendo il codice all'interno di `while` ciclo continuo:
    
    ```python
while True: red.on () sleep (1) amber.on () sleep (1) green.on () sleep (1) red.off () sleep (1) amber.off () sleep (1) verde. off ()
```

4. Ora sai come controllare le luci individualmente e cronometrare le pause tra i comandi, puoi creare una sequenza di semafori? La sequenza va:

- Verde acceso
- Ambra
- Rosso acceso
- Rosso e ambra
- Verde acceso

È importante pensare ai tempi. Per quanto tempo dovrebbero rimanere accese le luci in ogni fase?

Una volta completata la sequenza dei semafori, potresti provare ad aggiungere un pulsante e un cicalino per creare una versione interattiva.