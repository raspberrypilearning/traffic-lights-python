## Control the LEDs

1. Open Python 3 from the main menu, and open a new file.

2. Enter the following code:
    
    ```python
from gpiozero import LED

red = LED(22)

red.blink()
```

3. Now save your program and press **F5** to run your code. You should see the red light flash on and off continuously.

4. Now modify your code to introduce the other two lights, and make them blink at different speeds:
    
    ```python
from gpiozero import LED

red = LED(22)
amber = LED(27)
green = LED(17)

red.blink(1, 1)
amber.blink(2, 2)
green.blink(3, 3)
```

5. Run your code again and you should see the three lights flashing at different rates.

6. If a larger number makes a light blink slower, what number would make it run faster? Try to make your lights blink faster.