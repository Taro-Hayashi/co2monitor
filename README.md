# CO2モニター自作キット
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [組み立て](#組み立て)
- [カスタマイズ](#カスタマイズ)
- [その他](#その他)

## キット内容
![](img/IMG_1757.jpeg) 
||部品名|数| |
|-|-|-|-|
|1|メインボード|1||
|2|トッププレート|1||
|3|ボトムプレート|1||
|4|スタンド|1||
|5|スペーサー（短）|4||
|6|スペーサー（長）|2||
|7|ねじ|6||
|8|リセットスイッチ|1||
|9|LED|1||
|10|OLED|1||
|11|ピンソケット|1||
|12|キースイッチ|1||
|13|キーキャップ|1||
|14|ゴム足|6||

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|Pro Micro|1||
|MG-812使用CO2ガスセンサアンプキット|1|[秋月電子通商](https://akizukidenshi.com/catalog/g/gK-16446/)|
|USB ケーブル|1||

### 必要な工具
|工具名|
|-|
|はんだごて|
|こて先クリーナー（こて台）|
|鉛入りはんだ|
|精密ドライバー|
|ニッパー等ダイオードの足を切れるもの|
|エポシキ接着剤|
|Microsoft Edge、もしくはGoogle Chrome||

### あると便利な工具
|工具名|
|-|
|耐熱シリコンマット|
|温度調節可能なはんだごて|
|斜めに切ったタイプのこて先|
|フラックス|
|フラックスリムーバー、IPA|
|ピンセット|
|マスキングテープ|
|耐熱絶縁テープ（カプトンテープ）|
|テスター|
|はんだ吸い取り線|
|はんだ吸い取り器|



## 準備
Pro MicroはMicro-USB端子がもげやすいのでお好みでエポシキ接着剤で補強します。  
![](img/IMG_1011.jpeg)  
両サイドと手前側のはんだ付けされてるところに少し厚めに塗ります。端子の中に入り込まないように気を付けます。
![](img/IMG_1020.jpeg)  
乾燥させている間にはんだ付けを進めましょう。  

  
## はんだ付け
LEDをはんだ付けします。


### 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キットのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。  

Remapを使ってファームウェアの更新ができない場合は、QMK Toolboxをお試しください。  
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

### ロータリーエンコーダーのはんだ付け
表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/IMG_1887.jpeg)  

ツメを穴に引っかけてからピンを穴に差し込みます。
ピンを曲げてしまわないように注意してください。
![](img/IMG_1895.jpeg)   

差し込めたらはんだ付けします。
![](img/IMG_1901.jpeg)   

表からダイヤル型のロータリーエンコーダーを取り付けて裏からはんだ付けします。
![](img/IMG_1904.jpeg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/IMG_1905.jpeg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。  

メインボードのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/IMG_1928.jpeg)   
ここの2箇所は表側はネジではなくスペーサー（中）で止めます。
![](img/IMG_1923.jpeg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/IMG_1937.jpeg)  
ゴム足も取り付けました。
![](img/IMG_1940.jpeg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/IMG_1948.jpeg)  

キーキャップとノブをつけて完成です。  
![](img/IMG_1951.jpeg)  

先ほどと同様の手順で本番用のファームウェアに更新しましょう。  
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

![](img/remap06.jpg)  

## カスタマイズ
このキットはレイヤー機能を使っています。  
![](img/layout.jpg)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/2fe2023fd6a9318985b9c40c264c6cef)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  

ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/

![](img/remap1.png)  
左を選んで進んでいくとアドレスバーからメッセージが出てキーボードを選択できます。  

ドラッグアンドドロップでキーマップの変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  

### 置く向きに合わせる
レイアウトオプションから方向を変えることができます。  
![](img/c.jpg)  

### レイアウトの保存と復元
⇔アイコンで作ったレイアウトを保存することができます。  
いくつかサンプルをご用意しました。自分のレイアウトを公開することもできるので是非お試しください。
![](img/re.jpg)  

## その他
### Bluetooth接続
- [BLE Micro Pro使用例](ble.md)

### ぱいとん様のゆっくり実況動画  
ユーザーの方が組み立ての手順をとてもわかりやすく動画にしてくださいました。   
ご購入の前に雰囲気を掴んだり、ビルドガイドと一緒に見ながら作業するとわかりやすいと思いますのでぜひご覧ください。  
[![](http://img.youtube.com/vi/m9hnfXNCipo/0.jpg)](https://www.youtube.com/watch?v=m9hnfXNCipo)  

### ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/cannonball

### VIA用JSONファイル
- [cannonball.json](https://github.com/Taro-Hayashi/Cannonball/releases/download/15.20/cannonball.json)  

### プレートのデザインデータ  
[cannonball_plates.zip](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.31/cannonball_plates.zip)  
発注先のルールに沿ってデータを修正してください。  

### 謝辞
foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  

plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。

### 販売サイト
- 遊舎工房: https://shop.yushakobo.jp/collections/keyboard/products/2797   
- BOOTH: https://tarohayashi.booth.pm/items/3172502
