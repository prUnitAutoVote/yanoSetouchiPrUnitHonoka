# 瀬戸内PR部隊Season2 矢野帆夏自動投票プログラム ※劇場盤シリアルコードのみ

### 概要
「STU48瀬戸内PR部隊 Season2」の投票画面で自動で「矢野帆夏」に投票するツールです。  
Go言語の`chromedp`というライブラリで作成しました。`chromedp`はGoogle Chromeを自動操作するパッケージです。  
そのため、当プログラムを使用するにはGoogle Chromeのインストールが必要ですので、ご留意ください。
 
### 各ファイルについて 
- シリアルコード.txt: 投票シリアルコードのリスト。シリアルコードごとに改行すること。[作成方法](https://twitter.com/OBJ_ORIENTED46/status/1511239654611165185)  
- 都道府県.txt: 「全国ツアーを開催してほしい都道府県を1つお選びください」欄で入力する都道府県。**「都」「道」「県」「府」までフルで入力すること。** [記載例](https://twitter.com/OBJ_ORIENTED46/status/1511527524114702342)  
- yanoSetouchiPrUnitHonoka.exe: 自動投票プログラム本体  
- シリアルコード_XXXXX.jpg: 確認画面のスクショ。投票が完了するたびにscreenshotsフォルダ内に作成される。
- 使用済みシリアルコード.txt: 投票済みのシリアルコード。ツール実行中は開かないこと。 ※排他で書き込めなくなるためツールが止まる


### 使い方
1. プロジェクトごとダウンロードする
2. inputフォルダの「シリアルコード.txt」にシリアルコードを記載する(１シリアルコードごとに改行)
3. inputフォルダの「都道府県.txt」に入力したい都道府県を記載する(1行目に記載すること)
4. yanoSetouchiPrUnitHonoka.exeをダブルクリックで実行 ※Macの人はyanoSetouchiPrUnitHonoka

### 動作確認済み環境
端末： MacBook Air (M1, 2020)  
OSバージョン: macOS Monterey version 12.2.1  
プロセッサ: Apple M1  
Chromeバージョン: 99.0.4844.83（Official Build） （arm64）
  
端末： GALLERIA ZA9C-R38  
OSバージョン: Winodws 10 Home  
プロセッサ: Intel Core i9-10850K  
Chromeバージョン:99.0.4844.84(Official Build)(64ビット)  
