## Control the LEDs

\--- task \---

Open **Mu** from the main menu.

\--- /task \---

\--- task \---

Enter the following code:

```python
from gpiozero import LED

red = LED(22)

red.blink()
```

\--- /task \---

\--- task \---

Now save your program and press **F5** to run your code. You should see the red light flash on and off continuously.

\--- /task \---

\--- task \---

Now modify your code to introduce the other two lights, and make them blink at different speeds:

```python
from gpiozero import LED

red = LED(22)
amber = LED(27)
green = LED(17)

red.blink(1, 1)
amber.blink(2, 2)
green.blink(3, 3)
```

\--- /task \---

\--- task \---

Run your code again and you should see the three lights flashing at different rates.

\--- /task \---

\--- task \---

If a larger number makes a light blink slower, what number would make it run faster? Try to make your lights blink faster.

\--- /task \---