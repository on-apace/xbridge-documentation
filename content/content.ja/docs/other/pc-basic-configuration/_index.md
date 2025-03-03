# ホストの PC の基本設定

xBridge のアカウント所有者であるホストが会議を開始している間のみ、参加者やスピーカーがご利用いただけます。
そのため、会議中には継続して会議を利用している状態にする必要があります。
PC のスリープやスクリーンセーバーなどに機能により、予期せず PC が機能を停止し xBridge の会議が終了されないようにしてください。

## 1.電源を PC へ接続

電源タップを PC に必ず接続し、会議中に電源が切れないようにしてください。

## 2.音声入力設定

ご利用の PC のデフォルトマイクを通訳元の音声として選択します。  
そのため、PC の設定からデフォルトの音声を選択してください。

### 2-1.MAC での音声入力設定

`システム設定`→`サウンド`の`出力と入力`欄から`入力`を選択して、音声デバイスを指定してください。音声を実際に入力すると`入力レベル`のゲージが反応します。

{{< figure src="images/mac-sound-configuration.png" class="center" >}}

### 2-1.Windows での音声入力設定

`システム`→`サウンド`の`入力`欄から音声デバイスを指定してください。

{{< figure src="images/windows-sound-configuration.png" class="center" >}}

## 3.スリープ防止

会議中　 PC のスリープはしないように設定してください。

### 3-1.MAC スリープ防止

`システム設定`→`ロック画面`にて、以下の項目を設定してください。

1.  `使用していない場合はスクリーンセーバを開始`：しない
2.  `バッテリー駆動時に仕様していない場合はディスプレイをオフにする`：しない
3.  `電源アダプタ駆動時に使用していない場合はディスプレイをオフにする`：しない

{{< figure src="images/mac-sleep-configuration.png" class="center" >}}

### 3-2.Windows スリープ防止

`システム`→`電源とバッテリー`の`電源`欄にて以下の項目を設定してください。

1.  `バッテリー駆動時に、次の時間が経過したあとに画面の電源を切る`：なし
2.  `電源接続時に、次の時間が経過したあとに画面の電源を切る`：なし
3.  `バッテリー駆動時に、次の時間が経過したあとにデバイスをスリープ状態にする`：なし
4.  `電源接続時に、次の時間が経過したあとにでデバイスをスリープ状態にする`：なし

{{< figure src="images/windows-sleep-configuration.png" class="center" >}}
