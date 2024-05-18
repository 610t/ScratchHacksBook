# Scratch Hacks!!

[Scratchと遊ぼう:NT山城版](https://scrapbox.io/610t/Scratch%E3%81%A8%E9%81%8A%E3%81%BC%E3%81%86:NT%E5%B1%B1%E5%9F%8E%E7%89%88)

## はじめに
みなさん、Scratchはご存知ですか?
ブロックを積み重ねてプログラムを創るScratchは、ひょっとしたら学校や[CoderDojo](https://coderdojo.jp/)などで使ったことがあるかもしれません。

本書では、Scratchの基礎などについては、一切説明しません。
良書がたくさんでているので、それらを参考にしてくだい。

私が初めてScratchと出会ったのは、「Scratch: A Sneak Preview」という論文を読んだことでした。
この時は、まだアルファ版で、今とはかなり雰囲気の異なる環境になっています。
この論文ではあまりそのスゴさ理解できていなかったのが、私の先見の明がなかったところです。

当時は、[Squeak](https://squeak.org/)というブロックプログラミングに似たタイルスクリプティングベースの環境で遊んでいました。
C5という京都大学で行われていた国際会議なども定期的に行われており、Squeakに関連した人たちが多く参加していました。

Squeakの時代から、その言語環境内で閉じるのではなく、外部のデバイスと一緒に使う試みがたくさんありました。
Scratchの場合は公式拡張機能を使ってLEGOシリーズやmicro:bitと一緒に使えることを知っている人も多いかもしれません。
こういうデバイスと一緒にScratchを使うことは、私には大好物です。

本書ではこれらを踏まえて、Scratchの少し(?)変わった使い方の紹介をします。

以下のようなデバイスやサービスをScratchと一緒に使用します。

デバイスとしては、以下のようなものを使用します。
各デバイスの詳しい使い方についても、もうしわけありませんが、本書では説明しません。
動作に必要な最低限の説明だけを行います。
- M5Stack
  - ｽﾀｯｸﾁｬﾝ
- micro:bit
- AkaDako
- hapStak
- Seeeduino XIAOシリーズ, WioTerminal

また、以下のようなサービスを利用します。
- IFTTT
- [not yet]ChatGPT(ChatGPT2Scratch)
- [not yet]TeachableMachine(TM2Scratch, TMPose2Scratch)
- [not yet]音声認識(Speech2Scratch)
- [not yet]画像分類器(ImageClassifier2Scratch)
- [not yet]ポーズ認識(Posenet2Scratch, Facemesh2Scratch, Handpose2Scratch)

みなさんのScratchライフが楽しいものになれば筆者としてはうれしいです。

Happy Scratch Hacking!!

## Scratchってなぁに?
[Scratch](https://scratch.mit.edu/)

## Scratch拡張機能

## 拡張機能最強サーバーStretch3
[Stretch3](https://stretch3.github.io/)

### Microbit More
[Microbit More](https://microbit-more.github.io/)

[micro:bit](https://microbit.org/)

### AkaDako
[AkaDako](https://akadako.com/)

#### 参考文献
- [ビジュアルプログラミングでブルブルブルッ](https://scrapbox.io/M5S/%E3%83%93%E3%82%B8%E3%83%A5%E3%82%A2%E3%83%AB%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%9F%E3%83%B3%E3%82%B0%E3%81%A7%E3%83%96%E3%83%AB%E3%83%96%E3%83%AB%E3%83%96%E3%83%AB%E3%83%83):AkaDakoとhapStakを使って、入力でブルブル震えるシステムを作ってみました。

### IFTTT
[IFTTT](https://ifttt.com/)

## M5Stackと遊ぼう!!
[M5Stack](https://m5stack.com/)

### M5Stackってなぁに?
M5Stackは、色々な機能が一つになった、とても便利なマイコンデバイスです。

M5Stackには、機種によって違いますが、以下のような機能があります。
各機種のリンクは、日本の正規代理店のひとつであるスイッチサイエンスの販売ページになっています。
- CPU:		ESP32C, ESP32S, K210など
- ディスプレイ:320x240TFT([Core](https://www.switch-science.com/products/9010),[Core2](https://www.switch-science.com/products/6530),[CoreS3](https://www.switch-science.com/products/8960)), 80×160TFT(M5StickC), 135x240TFT([C Plus](https://www.switch-science.com/products/6470),[C Plus2](https://www.switch-science.com/products/9350)), 240 x 135TFT([Cardputer](https://www.switch-science.com/products/9277)), 5x5フルカラーLED([ATOM Matrix](https://www.switch-science.com/products/6260))
- バッテリー:	150mAh(Core), 390mAh(Core2), 500 mAh(CoreS3), 80or95mAh(C), 120mAh(C Plus), 120 mAh+1400 mAh(Cardputer)
- ネットワーク:Wi-Fi(2.4G) + BLE
- センサー:	加速度センサー、ジャイロ、ボタンスイッチ、温度センサーなど
- オーディオ:	マイク, スピーカー
- カメラ:		30万画素
- その他I/O:	Grove A(I2C), B(A/D,GPIO), C(UART), M-BUSなど
- 付属品:		キーボード、腕時計バンド、LEGOマウント

初めて買うときの私のおすすめは、[M5StickC Plus2 ウォッチアクセサリキット](https://www.switch-science.com/products/9420)です。
腕に巻いて遊べます!!

ただ、後で説明するｽﾀｯｸﾁｬﾝで遊びたい場合は、現状ではCore2シリーズ(Core2, [Core2aws](https://www.switch-science.com/products/6784))を買っておいた方が良いです。

### M5StackとScratchで遊ぶための参考文献
- [M5StackとScratchで遊ぶたった3つの冴えたやり方](https://scrapbox.io/M5S/M5Stack%E3%81%A8Scratch%E3%81%A7%E9%81%8A%E3%81%B6%E3%81%9F%E3%81%A3%E3%81%9F3%E3%81%A4%E3%81%AE%E5%86%B4%E3%81%88%E3%81%9F%E3%82%84%E3%82%8A%E6%96%B9):M5StackとScratchで遊ぶためのUIFlow, M5Scratch, M5bitLessの3(+1)つの方法について解説しています。
- [ScratchとM5Stackで遊ぶ](https://scrapbox.io/M5S/Scratch%E3%81%A8M5Stack%E3%81%A7%E9%81%8A%E3%81%B6):Scratch遠隔センサーについての説明が少し詳しめです。

### M5bitLess: M5StackでMicrobit Moreを使う

#### 参考文献
- [M5bitLess: M5Stack x Scratch3 = So Fun!!](https://protopedia.net/prototype/2395):M5bitLessのシステム全体を知るのに良いと思います。
- [M5bitLess label & data extension](https://protopedia.net/prototype/3224):データをやり取りするLabelとDataというしくみの説明です。
- [M5bitLessのI/Oサポート](https://protopedia.net/prototype/3821):M5bitLess外部のハードウエアを利用するための拡張についての説明です。
- デモ類
  - [M5StackとScratchとhapStakでスポーツの秋に挑戦!!](https://protopedia.net/prototype/2549):M5bitLessを使って、運動するゲームを作ってみました。

#### その他のボードで*bitLess系列を使う

- Seeeduino XIAOシリーズ (ESP32C3, nRF52480(Sense)):  [XIAO32bitLess](https://github.com/610t/XIAO32bitLess)
- Seeeduino WioTerminal:  M5bitLessに対応コードあり
- IoT Algyan [XIAOGYAN](https://github.com/algyan/XIAOGYAN):  [XIAOGYANbitLess](https://github.com/610t/XIAOGYANbitLess)

##### 参考文献
- [いろんなボードからScratchを使おう](https://scrapbox.io/M5S/%E3%81%84%E3%82%8D%E3%82%93%E3%81%AA%E3%83%9C%E3%83%BC%E3%83%89%E3%81%8B%E3%82%89Scratch%E3%82%92%E4%BD%BF%E3%81%8A%E3%81%86):色々なボードでScratchを使っている例です。

### Scratch1.4 遠隔センサープロトコル
#### Scratch 1.4
[Scratch 1.4](https://scratch.mit.edu/scratch_1.4)

##### 遠隔センサープロトコル
[Remote Sensors Protocol](https://en.scratch-wiki.info/wiki/Remote_Sensors_Protocol)

#### M5Scratch = Scratch x M5Stack

#### 参考文献
- [M5Scratch: M5Stack x Scratch1.4](https://protopedia.net/prototype/5188):システム全体の説明です。すみません英語です。
- デモ類
  - [M5Scratchを使って、M5Scratchの仲間たちとScratchを使ったゲームを作ろう!!](https://elchika.com/article/29135dba-ac4d-4ed7-b6cb-e33750f52f6b/):M5Scratchでゲームを作ってみた例です。
  - [M5Stack Christmas with M5Scratch](https://www.hackster.io/610t/m5stack-christmas-with-m5scratch-1055a2):これもゲームを作ってみた例です。すみません英語です。

## スーパーかわいいロボットｽﾀｯｸﾁｬﾝ
[スタックチャン（Stack-chan）](https://protopedia.net/prototype/2345)は、ししかわさんが開発、公開している手乗りサイズのｽｰﾊﾟｰｶﾜｲｲコミュニケーションロボットです。
ｽﾀｯｸﾁｬﾝはオープンソースで開発されており、ハードウエア(サーボのドライバーや体(筐体)の3Dデザインなど)もソフトウエア(AI用やBluetoothスピーカ版など)もオープンなものがたくさん存在します。

ｽﾀｯｸﾁｬﾝには、様々な亜種が存在します。
例えば、ソフトウエア的にはAIが使えるバージョンやスピーカーになるバージョンがあります。
ハードウエア的には、タンク形状のものや、かなり小型化されたいるものなど実に多様です。
[みんなのｽﾀｯｸﾁｬﾝ作例集](https://okimoku.com/gallery/)に色々なｽﾀｯｸﾁｬﾝが紹介されています。
なんと、等身大で自律的に動く[スタックサン](https://protopedia.net/prototype/4058)というヒューマノイドまであります。

残念なことに、2024年5月時点では、これだけを買えばすぐに使えるというものは存在しません。
体(筐体)の種類もいろいろあり、動かすためのサーボモーターの種類や、M5Stackの機種による違いなどがあり、簡単に説明することができない状態です。
これは、将来的には解決されると思うのですが、こういう現状のためここではｽﾀｯｸﾁｬﾝの作り方については説明しません、というかできません。
AIｽﾀｯｸﾁｬﾝの作成方法に関しては、動画「[知識ゼロで作る！　手乗りサイズのｽｰﾊﾟｰｶﾜｲｲﾛﾎﾞｯﾄ　AIｽﾀｯｸﾁｬﾝ2PLUS版](https://www.youtube.com/watch?v=Tit3mTCMoYY)」を見ると作成作業の手順がつかめると思います。

ｽﾀｯｸﾁｬﾝは動きが素敵だと思うのですが、動かなくても良いと割り切れる場合はCore2またはCore2awsだけを使って、そのスゴさを確認することはできると思います。

### 音声入出力を使って遊ぼう
[ｽﾀｯｸﾁｬﾝとScratchﾁｬﾝ](https://protopedia.net/prototype/4967)

#### 参考文献
- [Scratch V2 Programming](https://scrapbox.io/610t/Scratch_V2_Programming):ｽﾀｯｸﾁｬﾝとhapStakを音声で使っています。

### M5bitLessを使って遊ぼう
[ｽﾀｯｸﾁｬﾝ meets Scratch with M5bitLess](https://protopedia.net/prototype/4957)

## Scratchサーバーを自分で立ち上げる

### 拡張機能を追加する

### 参考文献
- [Scratchサーバーを手元で立ち上げる](https://scrapbox.io/610t/Scratch%E3%82%B5%E3%83%BC%E3%83%90%E3%83%BC%E3%82%92%E6%89%8B%E5%85%83%E3%81%A7%E7%AB%8B%E3%81%A1%E4%B8%8A%E3%81%92%E3%82%8B):Scratchサーバーを自分で作るための概略説明です。
- [Scratch at FreeBSD](https://scrapbox.io/BSD/Scratch_at_FreeBSD):実際に[FreeBSD](https://www.freebsd.org/)というOSでサーバーを立ち上げた例です。他のOSでも参考になるかと思います。

## おわりに
