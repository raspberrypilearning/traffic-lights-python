## Vezéreld a LED-eket

\--- task \---

Indítsd el a **Mu**-t a főmenüből.

\--- /task \---

\--- task \---

Írd be az alábbi kódot:

```python
from gpiozero import LED

piros = LED(22)

piros.blink()
```

\--- /task \---

\--- task \---

Mentsd el a programot és nyomd meg az **F5**-öt, hogy futtasd a kódodat. Most láthatod, hogy a piros lámpa fénye folyamatosan ki-be kapcsol.

\--- /task \---

\--- task \---

Most változtass a kódodon: add hozzá a másik két lámpát, és állítsd be, hogy különböző sebességgel villogjanak:

```python
from gpiozero import LED

piros = LED(22)
sarga = LED(27)
zold = LED(17)

piros.blink(1, 1)
sarga.blink(2, 2)
zold.blink(3, 3)
```

\--- /task \---

\--- task \---

Futtasd újra a kódot, és látni fogod, hogy a három lámpa különböző sebességgel villog.

\--- /task \---

\--- task \---

Ha egy nagyobb szám a lámpa villogását lassítja, akkor milyen szám gyorsítja a fényeket? Próbáld meg gyorsítani a fények villogását.

\--- /task \---