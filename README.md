# CO2モニター自作キット
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [組み立て](#組み立て)
- [その他](#その他)

## ご注意
- CO2センサーは発熱するので低温やけどに注意ください。
- 表示される数値は正確な濃度ではありません。換気された部屋を400ppmとした目安の値です。
- データを公開しているのでご自分で発注することができます。

## キット内容
![](img/IMG_1757.jpeg) 
||部品名|数||
|-|-|-|-|
|1|メインボード|1||
|2|トッププレート|1||
|3|ボトムプレート|1||
|4|スタンド|1||
|5|スペーサー（短）|4|M2 6mm|
|6|スペーサー（長）|2|M2 9mm|
|7|ねじ|6|M2 6mm|
|8|リセットスイッチ|1||
|9|LED|1|SK6812MINI-E|
|10|OLED|1||
|11|ピンソケット|1||
|12|キースイッチ|1||
|13|キーキャップ|1||
|14|ゴム足|6||

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|Pro Micro（Micro-B or Type-C）|1||
|MG-812使用CO2ガスセンサアンプキット|1|[秋月電子通商](https://akizukidenshi.com/catalog/g/gK-16446/)|
|USB ケーブル|1||

### 必要な工具
|工具名|
|-|
|はんだごて|
|はんだ|
|精密ドライバー|
|ニッパー|
|エポシキ接着剤|

## はんだ付け
LEDをメインボード裏面にはんだ付けします。欠けがある方向と折れ曲がった白線が一致するようにしてください。

リセットスイッチを裏面から差し込みはんだ付けします。

ピンソケットを表面に差し込みはんだ付けします。

Pro Microを付属のピンヘッダーで取り付けて両面をはんだ付けします。

MG-812使用CO2ガスセンサアンプキットを写真のように組み立てます。

メインボードの表面に差し込みはんだ付けします。

付属、もしくはお好みのキースイッチを表面に差し込みはんだ付けします。

OLEDにピンヘッダを差し込みはんだ付けしたらメインボードに取り付けます。

はんだ付けが終わったら動作の確認をするためにUSBケーブルでPCと接続しましょう。

### 動作テスト
こちらのファイルをダウンロードしてファームウェアを書き込んでください。
- hex

こちらのサイトにGoogle ChromeでアクセスするとWebブラウザ経由で書き込むことができます。
- https://sekigon-gonnoc.github.io/promicro-web-updater/index.html

Chromeを使わない場合はQMK Toolboxを使ってファームウェアを書き込んでください。
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

ディスプレイに数字が表示され、キーを押すとLEDの発行方法が変わればはんだ付けに成功しています。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。  

メインボードにスペーサーを取り付けます。

表面の4箇所にスペーサー（短）を差し込み、裏面は写真のようにネジとスペーサー（長）で止めます。

ボトムプレートをねじで取り付けてゴム足を貼り付けたら完成です。

お好みでスタンドをお使いください。

### 使用方法
USBケーブルをPCやUSB充電器などに接続して好きなところに置いてください。  
起動した後に換気をすると正しい濃度に近い数値が表示されるようになります。


## その他
### ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/cannonball

### 発注用データ  
[cannonball_plates.zip](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.31/cannonball_plates.zip)    

### 販売サイト
- BOOTH: https://tarohayashi.booth.pm/items/4500742
