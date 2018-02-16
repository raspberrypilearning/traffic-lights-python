## 信号機のシーケンス

1. `on`関数でライトを点灯させることができます。 `sleep`関数を使って、処理を一時停止できます。 次の例では、ライトを順番に点灯します。
    
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

LEDのメインコントロールは、`on`、`off`、`toggle` `点滅`となります。

2. 順番にライトをオンまたはオフにしてみてください：
    
    ```python
red.on（）sleep（1）amber.on（）sleep（1）green.off（）sleep（1）red.off（）sleep（1）
```

3. `の中にコードを入れてこれを繰り返す`ループ：
    
    ```python
sleep（1）sleep（1）sleep（1）sleep（1）sleep（1）green.on（）sleep（1）red.onオフ（）
```

4. 今度は、ライトを個別に制御する方法を知り、コマンド間の休止時間を計る、信号灯シーケンスを作成することができますか？ シーケンスは次のようになります。

- グリーンオン
- アンバーオン
- レッドオン
- 赤と琥珀色
- グリーンオン

タイミングについて考えることが重要です。 各ステージでどれくらいの間ライトが点灯し続けるのですか？

信号灯のシーケンスを完了したら、ボタンとブザーを追加してインタラクティブなバージョンを作ってみてください。