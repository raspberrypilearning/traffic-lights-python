## 信号灯のシーケンス点灯

--- task ---

`on`関数でライトを点灯させることができます。 `sleep`関数を使って、処理を一時停止できます。 次のコードを実行して、ライトを順番に点灯させてみてください：

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

LEDの主な制御方法は、`on`(点灯)、`off`(消灯)、`toggle`(反転)と `blink`(点滅)になります。

--- /task ---

--- task ---

LEDを順番に点灯、消灯してみてください：

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

--- /task ---

--- task ---

このコードを`while`ループの中に入れて、処理を繰り返してみてください：

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

--- /task ---

--- task ---

これでLEDを個別に制御する方法と、点灯や消灯の時間を指定する方法が分かりましたね。では信号灯を決めた順番でつけたり消したりすることができますか？ 順番は次のとおりにします。

- 緑を点灯
- アンバーを点灯
- 赤を点灯
- 赤とアンバーを点灯
- 緑を点灯

タイミングについて考えることが重要です。 各順番でどれくらいの時間LEDを点灯させますか？

--- /task ---

信号灯のシーケンス作成を完了したら、ボタンとブザーを追加して、見るだけでなく操作できるバージョンも作りたくなるかもしれませんね。