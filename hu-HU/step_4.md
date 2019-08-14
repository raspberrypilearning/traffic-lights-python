## A közlekedési lámpa ciklusa

\--- task \---

Az `on` függvény bekapcsolja a lámpát. A `sleep` parancsot használhatod, hogy a szünetet tegyél két parancs közé. Próbáld ki ezt a példát, a lámpák sorrendben fognak bekapcsolni:

```python
from gpiozero import LED
from time import sleep

piros = LED(22)
sarga = LED(27)
zold = LED(17)

piros.on()
sleep (1)
sarga.on()
sleep (1)
zold.on()
sleep(1)
```

A LED-eket ezekkel a parancsokkal lehet vezérelni: `on`, `off`, `toggle` és `blink`. Az 'on' bekapcsolja, az 'off' kikapcsolja, a 'toggle' változtatja (ha be volt kapcsolva, ki kapcsolja; ha ki volt kapcsolva, bekapcsolja) és a 'blink' villogtatja a fényeket.

\--- /task \---

\--- task \---

Próbáld meg sorrendben ki-be kapcsolni a lámpákat:

```python
piros.on()
sleep(1)
sarga.on()
sleep(1)
zold.on()
sleep(1)
piros.off()
sleep(1)
sarga.off()
sleep(1)
zold.off()
```

\--- /task \---

\--- task \---

Próbáld ezt megismételni úgy, hogy belerakod a kódot egy `while` ciklusba:

```python
while True:
    piros.on()
    sleep(1)
    sarga.on()
    sleep(1)
    zold.on()
    sleep(1)
    piros.off()
    sleep(1)
    sarga.off()
    sleep(1)
    zold.off()
```

\--- /task \---

\--- task \---

Most, hogy már tudod, hogyan kell egyenként vezérelni a fényeket, és hogyan lehet szünetet rakni a parancsok közé, menni fog a jelzőlámpa? A fények sorrendje:

- Zöld bekapcsol
- Sárga bekapcsol
- Piros bekapcsol
- Piros és sárga bekapcsol
- Zöld bekapcsol

Fontos, hogy gondolj az időzítésre. Mennyi ideig világítsanak a fények a szakaszokban?

\--- /task \---

Miután befejezted a jelzőlámpát, hozzáadhatsz egy gombot és egy berregőt, így készíthetsz egy interaktív változatot.