## 信号灯のシーケンス

1. `on`関数でライトを点灯させることができます。 `sleep`関数を使って、処理を一時停止できます。 次のコードを実行して、ライトを順番に点灯してください：
    
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

LEDの制御は、`点灯`、`消灯`、`トグル`と `点滅`になります。

2. 順番にライトを点灯、消灯してみてください：
    
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

3. 上記の処理を`while`ループの中に入れて、処理を繰り返してみてください：
    
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

4. 次はライトを個別に制御する方法や、点灯や消灯の停止時間を把握しましょう。信号灯のシーケンスを作成することができますか？ シーケンスは次のようになります。

- 緑オン
- 琥珀オン
- 赤オン
- 赤と琥珀オン
- 緑オン

タイミングについて考えることが重要です。 各ステージでどれくらいの間ライトが点灯し続けるのでしょうか？

信号灯のシーケンス作成を完了したら、ボタンとブザーを追加して対話形式のバージョンを作ってみてください。
