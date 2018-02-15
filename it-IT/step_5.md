## La sequenza del semaforo

1. La funzione `on` ti permette di accendere una luce. È possibile utilizzare `sleep` per mettere una pausa tra i comandi. Prova questo esempio per accendere le luci in sequenza:
    
    ```python
from gpiozero import LED
from time import sleep

rosso = LED(22)
giallo = LED(27)
verde = LED(17)

rosso.on()
sleep(1)
giallo.on()
sleep(1)
verde.on()
sleep(1)
```

I controlli principali per i LED sono `on`, `off`, `toggle` e `blink`.

2. Prova ad accendere e spegnere in sequenza le luci:
    
    ```python
rosso.on()
sleep(1)
giallo.on()
sleep(1)
verde.on()
sleep(1)
rosso.off()
sleep(1)
giallo.off()
sleep(1)
verde.off()
```

3. Prova a ripetere questa sequenza inserendo il codice all'interno di un ciclo `while`:
    
    ```python
while True:
 rosso.on()
 sleep(1)
 giallo.on()
 sleep(1)
 verde.on()
 sleep(1)
 red.off()
 sleep(1)
 giallo.off()
 sleep(1)
 verde.off()
```

4. Ora sai come controllare le luci individualmente e come gestire le pause tra i comandi, puoi creare una sequenza di luci come quelle di un semaforo? La sequenza è questa:

- Verde acceso
- Ambra acceso
- Rosso acceso
- Rosso e ambra accesi
- Verde acceso

È importante pensare ai tempi. Per quanto tempo dovrebbero rimanere accese le luci in ogni fase?

Una volta completata la sequenza delle luci, potresti provare ad aggiungere un pulsante e un cicalino per creare una versione interattiva.