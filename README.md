# tab-a04-br3-edited-logo.img
Tab-a04-br3用logo.img(起動画面やrecovery起動する画面の画像ファイル入ったやつ)の改造版
起動時に表示されるbenesseを見なくするのに最適です
なんか起動画面のぼつ？みたいなやつはのこしてます
すべて画像は自分で作ってます。再配布禁止でご自由にお使いください！
# 場所
この文章の上にファイル載せてあります。originalが元logo.img。editedが編集後のlogo.img
中にimageとlogo.imgが入ってます
# FLASH方法
## MTKCLIENTを用いた方法
1.pythonとMTKCLIENTを導入する
2.windowsキー+Rを押してcmdと入力後、
```cd （c:\users/ownerなどのmtkclientファイルまでのパス）```へ移動する
3.タブレットシャットダウン後、これを実行して、__音量＋ボタンを長押しした状態__でパソコンとUSBをつなぐ。
この時、プログレスバーが出るまで長押ししたままにする。
```python mtk.py w --noreconnect logo (logo.imgまでのフルパス)```
4.USB抜いて再起動後、BENESSE表示なくなってることを確認！

## FASTBOOT使った方法(ADB導入済を想定)
1.タブレットを起動したまま、これを実行
```adb reboot bootloader```
2.画面が黒い画面のまま光っていることを確認。そしたらこれを実行
```fastboot flash logo (logo.imgまでのパス)```
3.ログがすべて出力されたらUSB抜いて電源切って再起動。
4.USB抜いて再起動後、BENESSE表示なくなってることを確認！

## UPDATE.zip使った方法
1.SDカードの最上のパスにupdate.zipを書き込む
2.ちゃれぱに刺す
3.設定→端末情報→システムアップデートを実行
4.再起動してbenesse表示なければ成功
これで失敗したとしても作者は責任を負いません。質問はdiscord:high28dawa X:high28hutabaまで！！
