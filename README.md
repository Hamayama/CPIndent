# CPIndent

![image](image.png)

## 概要
- C プリプロセッサの命令のインデント変換を行う HTML です。

- C のプログラム内で、C プリプロセッサの命令は、通常 インデントされないため、  
  `#if` 等の適用範囲が分かりにくい場合があります。  
  本アプリは、この適用範囲を分かりやすく確認するための簡易ツールです。  
  (基本的に確認専用です)

- 実行例は、以下のページにあります。  
  https://hamayapp.appspot.com/static/cpindent.html


## 使い方
- cpindent.html を ブラウザで開くと起動します。

- src のテキストボックスに C のプログラムを貼り付けて、  
  convert ボタンをクリックすると、C プリプロセッサの命令のインデント変換を実行します。  
  結果は、out のテキストボックスに表示されます。  
  また、その下にはブロックごとに色分けした結果も表示されます。

- initial indent のテキストボックスに数値を入力すると、変換時の初期インデント量を設定できます。

- また、color のチェックボックスのチェックを外すと、画面下部の表示で、色を付けなくなります。

- また、block no. のチェックボックスにチェックを入れると、画面下部の表示で、  
  `#` のところにブロック番号を表示します。  

- また、all のチェックボックスにチェックを入れると、C のプログラムも全てインデントします。  
  チェックを入れなければ、C プリプロセッサの命令のみインデントします。

- clear ボタンをクリックすると、入出力をすべてクリアします。

- sample1-3 ボタンをクリックすると、変換の例を表示します。

- 変換を実行しても変化がなかった場合には [ no change ] と表示します。


## 注意事項
1. インデントの単位は、半角スペース 4 個に固定です。

2. インデント変換は、#if 等のブロック内に半角スペースを追加するのみです。  
   このため、元々変なインデントになっている場合には うまく整形できません。


## 環境等
- OS
  - Windows 10 (version 1909) (64bit)
- ブラウザ
  - Chrome v87

## 履歴
- 2017-1-9   v1.00 (初版)
- 2017-1-9   v1.01 allのチェックボックス追加
- 2017-1-10  v1.02 サンプル修正
- 2017-1-10  v1.03 トークン分割処理一部見直し
- 2017-1-11  v1.04 トークン分割の正規表現修正
- 2017-1-11  v1.05 コメント修正のみ
- 2017-1-13  v1.06 改行のみの行はインデントしないように変更
- 2017-1-14  v1.07 コメント修正のみ
- 2017-4-18  v1.08 文字列の解析処理見直し等
- 2017-6-6   v1.09 コメント修正のみ
- 2017-7-17  v1.10 書式修正等
- 2018-6-26  v1.11 HTML見直し
- 2018-6-27  v1.12 HTML出力見直し(IE8対策)
- 2018-6-30  v1.13 HTML見直し
- 2020-12-9  v1.14 空白文字列作成処理見直し


(2020-12-9)
