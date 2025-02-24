# 多要素認証の設定

メニュ`設定`から`MFA AUTHENTICATION`タブをクリックしてください。
MFA スイッチをクリックし有効にし、登録用の QR コードが表示されます。

{{< figure src="images/2fa.png"  class="center" >}}

登録用の QR コード画面に表示される QR コードを Google Autheniticator などへ登録してください。
有効な OTP コードを入力し、`CONFIRM OTP`ボタンをクリックし OTP の確認を実施します。
有効な OTP が確認されれば、自動的にモーダルが消え多要素認証の有効化は完了です。
次回ログイン時に OTP の入力が求められます。
＊削除した場合ログインが出来なくなりますため、必ず多要素認証端末に登録した情報は削除しないでください。

{{< figure src="images/2fa-otp-code.png"  class="center" >}}
