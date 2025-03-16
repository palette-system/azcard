# ビルドガイド

## １．用意が必要な物

| 名前 | 詳細 | 個数 |
| --- | --- | --- |
| XIAO ESP32S3 | <a href="https://akizukidenshi.com/catalog/g/gM-18078/" target="_blank">秋月電子リンク</a> | 1 |
| キースイッチ | Kailh PG1316S<br><a href="https://holykeebs.com/products/kailh-pg1316s-butterfly-switch-10-pack">holykeebsリンク</a> | 12 |
| キーキャップ | Kailh PG1316 Keycaps<br><a href="https://holykeebs.com/products/kailh-pg1316s-keycaps">holykeebsリンク</a> | 12 |
| フルカラーLED | WS2812C-2020<br><a href="https://akizukidenshi.com/catalog/g/g115068/" target="_blank">秋月電子リンク</a> | 12 |
| ダイオード | 1N4148W<br><a href="https://akizukidenshi.com/catalog/g/g107084/" target="_blank">秋月電子リンク</a><br><a href="https://shop.yushakobo.jp/products/a0800di-02-100" target="_blank">遊舎工房リンク</a><br> | 12 |
| 木工用ボンド | コクヨ KOKUYO ボンド 木工用速乾<br><a href="https://www.yodobashi.com/product/100000001001555306/" target="_blank">ヨドバシカメラリンク</a> | 1 |

<br><br>

## ２．入っている物
![in_parts](/docs/img/make_31.jpg)

| 名前 | 詳細 | 個数 |
| --- | --- | --- |
| PCB | 　 | 1 |
| トッププレート | アルミ 0.8mm厚 | 1 |
| ミドルプレート | 透明アクリル 1.5mm厚 | 1 |
| 黒ネジ | M2 3mm | 6 |
| スペーサー | MAC8 TH-0.8-1.5-M2-B M2 1.5mm | 4 |

<br><br>

## ３．フルカラーLED のはんだ付け
フルカラーLEDのはんだ付けを写真の通りの向きで各スイッチ部分にLEDをはんだ付けして下さい。<br>
LEDの位置が左右に寄ってしまうと、LEDパッド裏のVCC、GNDなどが接触してしまいキーボードが動かなくなってしまうので、位置をパッドの中央になるよう注意して下さい。<br>
※フルカラーLEDが付いていなくてもキーボードして認識するので、はんだ付けに自身の無い方は付けない事をおススメします。<br>
![pic](/docs/img/make_01.jpg)
![pic](/docs/img/make_02.jpg)
<br><br>

## ４．ダイオード のはんだ付け
ダイオードのはんだ付けを写真の通りの向きではんだ付けして下さい。<br>
![pic](/docs/img/make_03.jpg)
<br><br>

## ５．XIAO ESP32S3 のはんだ付け
トッププレート、ミドルプレート、PCBを重ねて裏向きに置いて、裏から XIAO ESP32S3 をはんだ付けして下さい。<br>
![pic](/docs/img/make_04.jpg)
![pic](/docs/img/make_05.jpg)
![pic](/docs/img/make_06.jpg)
<br><br>

## ６．LEDとスイッチの動作確認
Chromeで下記リンクを開き、手順に従って動作確認用ファームウェアを書き込んでください。<br>
<a href="#">ファームウェア書き込みサイト</a><br>
<br>
書き込んだらスイッチ部分をピンセットでショートさせて、ボタンの部分のLEDが点灯する事を確認して下さい。<br>
![pic](/docs/img/make_07.jpg)
![pic](/docs/img/make_08.jpg)
<br><br>

## ７．PCBにスイッチを差し込む
PCBとスイッチの間に隙間ができないようにパチッと音が鳴るまでPCBにスイッチを差し込んで下さい。<br>
![pic](/docs/img/make_09.jpg)
![pic](/docs/img/make_10.jpg)
![pic](/docs/img/make_11.jpg)
<br><br>

## ８．スイッチ表面のはんだ付け
表面のスイッチの四つ角をはんだ付けしてスイッチを固定して下さい。<br>
PCBとスイッチの間に隙間ができてしまわない様注意しながらはんだ付けして下さい。<br>
![pic](/docs/img/make_12.jpg)
<br><br>

## ９．スイッチ裏面のはんだ付け
裏面からスイッチのロジック分のはんだ付けを行います。<br>
裏面の穴からスイッチのパッド部分にはんだごてをあてて、スイッチの金属パッドが温まった所にはんだを少量流し込むとうまくはんだ付けできます。<br>
この時はんだを流し込みすぎてしまうと、はんだがスイッチ内の方まで流れてスイッチの接触不良につながってしまうためはんだを流し込み過ぎない様気を付けて下さい。<br>
![pic](/docs/img/make_13.jpg)
![pic](/docs/img/make_14.jpg)
![pic](/docs/img/make_15.jpg)
![pic](/docs/img/make_16.jpg)
<br><br>

## １０．スイッチの接触確認
USBを接続してスイッチが押されるとLEDが光る事を確認して下さい。<br>
![pic](/docs/img/make_17.jpg)
<br><br>

## １１．スペーサーのはんだ付け
PCBの四つ角にスペーサーを差し込み、周りをはんだ付けして下さい。<br>
この時はんだが多すぎるとミドルプレートがはまらなくなってしまうためはんだを付け過ぎない様気を付けて下さい。<br>
![pic](/docs/img/make_18.jpg)
![pic](/docs/img/make_19.jpg)
<br><br>

## １２．裏面にボンドを塗って絶縁
PCBの裏面に木工用ボンドを塗り、たまたま家に余っていたESP32などを使用してボンドを全体に塗り伸ばして下さい。<br>
ボンドが固まるまでそのまま乾かして下さい。<br>
![pic](/docs/img/make_28.jpg)
![pic](/docs/img/make_29.jpg)
![pic](/docs/img/make_30.jpg)
<br><br>

## １３．AZCARDキーボードのファームウェアの書き込み
Chromeで下記リンクを開き、手順に従って動作確認用ファームウェアを書き込んでください。<br>
<a href="#">ファームウェア書き込みサイト</a><br>
<br>
![pic](/docs/img/make_18.jpg)
<br><br>

## １４．プレートの固定
ミドルプレートの保護シートをはがしてPCBにミドルプレート、トッププレートを重ねて下さい。<br>
重ね終わったら四つ角にネジをとめて固定して下さい。<br>
![pic](/docs/img/make_20.jpg)
![pic](/docs/img/make_21.jpg)
![pic](/docs/img/make_22.jpg)
![pic](/docs/img/make_23.jpg)
<br><br>

## １５．スイッチキャップを付ける
写真を参考に上側をひっかけて押し込むとキャップがスイッチに固定できます。<br>
![pic](/docs/img/make_24.jpg)
![pic](/docs/img/make_25.jpg)
![pic](/docs/img/make_26.jpg)
![pic](/docs/img/make_27.jpg)
<br><br>

## １６．ゴム足を付ける
裏面にゴム足を付けて完成です。<br>
![pic](/docs/img/make_32.jpg)

