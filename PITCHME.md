# Webサイトの概要
---
## Webページを構成する要素
---
### クライアント
1. ブラウザ
	1. HTML
	2. CSS
	3. JavaScript
	4. 画像
	5. 動画

などなど

---
### サーバ
1. Webサーバ
2. DNSサーバ
---
### 通信方法（プロトコル）
1. HTTP
---
## Webページが表示されるまで
ブラウザ  
（URLの問い合わせをする）  
　↓  

+++

DNSサーバ  
（URLのIPアドレスが送られてくる）  
　↓  

+++

ブラウザ  
（送られてきたIPを持つサーバへデータのリクエストをする）  
　↓  

+++

サーバ  
（リクエストしたデータが送信されてくる）  
　↓  

+++

ブラウザ  
（レンダリング）

**これを繰り返してユーザーが見る画面が作成される**

参考：[HTML初心者必見！Webページの仕組みをわかりやすく説明！](https://blog.codecamp.jp/html_web_base)

---
## ブラウザについて
1. Windows Google Chrome / Firefox / Internet Explorer / Edge
3. Mac Google Chrome / Firefox / Safari
6. iOS Safari / Chrome
8. Android ブラウザ / Chrome

いろいろある！！

参考：[ウェブブラウザ](https://ja.wikipedia.org/wiki/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%96%E3%83%A9%E3%82%A6%E3%82%B6)  
参考：[ウェブブラウザの一覧](https://ja.wikipedia.org/wiki/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%96%E3%83%A9%E3%82%A6%E3%82%B6%E3%81%AE%E4%B8%80%E8%A6%A7)

---
## HTMLとCSSの関係性
1. HTMLは文章の定義をし、CSSはそれを装飾する
2. HTMLとCSSにはそれぞれバージョンがあるが、どのバージョンが使えるかはブラウザに依存する
3. HTML5じゃないとCSS3が使えないなど勘違いする人がいるけど関係ない

---
## JavaScriptの役割と関わり方
HTMLやCSSでできないことを行う

1. アニメーション（CSSでも出来るが複雑なものは難しい）
2. ユーザーのアクションに合わせたイベントの実行
3. ブラウザの情報取得
4. HTML要素の情報取得・変更

などなど

**HTML・CSSとの連携が必須**