## LEDを制御する

\--- task \---

メインメニューから**Mu**を開きます。

\--- /task \---

\--- task \---

以下のコードを入力します。

```python
from gpiozero import LED

red = LED(22)

red.blink()
```

\--- /task \---

\--- task \---

ファイルを保存し、**F5**キーを押してコードを実行します。 赤いライトが連続的に点滅するはずです。

\--- /task \---

\--- task \---

さらに他の2つのLEDも使えるようにコードを追加し、それらのLEDが異なる速度で点滅するようにします。

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

もう一度コードを実行すると、3つのライトが異なる速度で点滅します。

\--- /task \---

\--- task \---

大きい数字の指定でLEDの点滅が遅くなるなら、点滅を速くするにはどのような数字を指定すればよいでしょう？ LEDの点滅を速くするようにしてみましょう。

\--- /task \---