## Traffic lights sequence

1. The `on` function allows you to turn a light on. You can use `sleep` to pause between commands. Try this example to turn the lights on in sequence:

   ```python
   from gpiozero import LED
   from time import sleep

   red = LED(22)
   amber = LED(27)
   green = LED(17)

   red.on()
   sleep(1)
   amber.on()
   sleep(1)
   green.on()
   sleep(1)
   ```

   The main controls for LEDs are `on`, `off`, `toggle` and `blink`.

1. Try turning the lights on and off in sequence:

   ```python
   red.on()
   sleep(1)
   amber.on()
   sleep(1)
   green.on()
   sleep(1)
   red.off()
   sleep(1)
   amber.off()
   sleep(1)
   green.off()
   ```

1. Try repeating this by putting the code inside a `while` loop:

   ```python
   while True:
       red.on()
       sleep(1)
       amber.on()
       sleep(1)
       green.on()
       sleep(1)
       red.off()
       sleep(1)
       amber.off()
       sleep(1)
       green.off()
   ```

1. Now you know how to control the lights individually, and time the pauses between commands, can you create a traffic lights sequence? The sequence goes:

   * Green on
   * Amber on
   * Red on
   * Red and amber on
   * Green on

It's important to think about timing. How long should the lights stay on for at each stage?

Once you have completed the traffic lights sequence, you might want to try adding in a button and a buzzer to make an interactive version.
