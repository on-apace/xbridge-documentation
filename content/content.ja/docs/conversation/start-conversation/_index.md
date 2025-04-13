# 会議を開始

## 1.ホストの PC 設定

予期せぬ会議の終了などを防ぐため、[ホストの PC の基本設定]({{< relref "/docs/other/pc-basic-configuration" >}})を参考に、ホスト PC の設定をしてください。

## 2.会議を開始

会議詳細画面の右上 `OPEN ROOM`ボタンをクリックすることで会議を開始します。

{{< figure src="images/start-conversation.png" class="center" >}}

{{< figure src="images/started-conversation.png" class="center" >}}

{{< hint warning >}}
**通訳開始には 10-60 秒程度かかることがあります**  
会議開始後、数秒間は画面上部に`Conversation is closed`など赤字のエラーが表示され通訳のシステムが準備できるまで待ちます。
会議のモデルに「OpenAI Whisper」を選択している場合、開始できる状態なるまで最大 60 秒かかる場合があります。
{{< /hint >}}

スピーカーは別の端末から参加し、会話を開始してください。
自動的に、通訳結果が各端末へ表示されます。

ホストがスピーカーとなる場合、マイクボタンをクリックし有効にし会話を開始してください。有効の場合は赤色のマイクが表示されます。
通訳結果の音声読み出しをご利用になる場合は、スピーカーボタンをクリックし有効にしてください。有効の場合は、赤色のスピーカーが表示されます。
会議が終了したら、退出ボタンをクリックして必ず退出ください。

最新の更新通訳内容は青字でハイライトされます。

{{< columns >}}

{{< figure src="images/conversation-ex1.png"  class="center" >}}
ホストの言語は英語で、日本語スピーカーの通訳結果を表示。
英語の通訳結果が表示されます。

<--->

{{< figure src="images/conversation-ex2.png" class="center" >}}
ホストの言語は英語で、英語スピーカーの通訳結果を表示。
英語の書き起こし結果のみが表示されます。

{{< /columns >}}

## 3.会議設定変更

注意：会議中の設定変更は反映に時間がかかる場合があるため、推奨しておりません。
会議開催中の設定変更は追加設定アイコンをクリックします。
ポップアップメニューから `Mute All participants`と`Settings`が選択出来ます。
`Mute All participants`の有効化・無効化により、ホスト以外のスピーカーの発話を許可・拒否出来ます。

{{< figure src="images/popup-config.png" class="center" >}}

`Settings`ボタンをクリックし、会議のホストの言語設定変更や会議参加者の言語設定変更が可能です。
ホストの言語設定変更をする場合、メニューの`MY PROFILE`タブをクリックし、言語を選択してください。

{{< figure src="images/config-lang.png" class="center" >}}

Speaker と Viewer の言語設定変更をする場合、メニューの`BROADCAST`タブをクリックし、言語を選択してください。
選択後`REFRESH`ボタンをクリックして設定変更を反映します。
設定反映まで時間がかかることがございます。

{{< figure src="images/config-broadcast-langs.png" class="center" >}}
