# クリエイター本部向けコーディング研修 2017

---

## Webサイトの概要

---

### Webページを構成する要素

---

#### クライアント
1. ブラウザ
	1. HTML
	2. CSS
	3. JavaScript
	4. 画像
	5. 動画

などなど

---

#### サーバ
1. Webサーバ
2. DNSサーバ

---

#### 通信方法（プロトコル）
1. HTTP

---

### Webページが表示されるまで
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

### ブラウザについて
1. Windows Google Chrome / Firefox / Internet Explorer / Edge
3. Mac Google Chrome / Firefox / Safari
6. iOS Safari / Chrome
8. Android ブラウザ / Chrome

いろいろある！！

参考：[ウェブブラウザ](https://ja.wikipedia.org/wiki/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%96%E3%83%A9%E3%82%A6%E3%82%B6)  
参考：[ウェブブラウザの一覧](https://ja.wikipedia.org/wiki/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%96%E3%83%A9%E3%82%A6%E3%82%B6%E3%81%AE%E4%B8%80%E8%A6%A7)

---

### HTMLとCSSの関係性
1. HTMLは文章を定義し、CSSはそれを装飾する
2. HTMLとCSSにはそれぞれバージョンがあるが、どのバージョンが使えるかはブラウザに依存する
3. HTML5じゃないとCSS3が使えないなど勘違いする人がいるけど関係ない

---

### JavaScriptの役割と関わり方
**HTMLやCSSでできないことを行う**

1. アニメーション（CSSでも出来るが難しい場合がある）
2. ユーザーのアクションに合わせたイベントの実行
3. ブラウザの情報取得
4. HTML要素の情報取得・変更

などなど

**HTML・CSSとの連携が重要**

---

## HTMLコーディング

---

### HTMLタグについて

```
<h1>吾輩は猫である</h1>
<p>吾輩わがはいは猫である。名前はまだ無い。</p>
```

**<></>がHTMLタグと呼ばれるもの**

---

#### HTMLタグはたくさんある

参考：[HTML5要素一覧［ABC順］](http://www.tagindex.com/html5/elements/abc.html)

たくさんあるけど使用するのは一握りで、よく使われるものが

1. a
2. h1〜h6
3. p
4. ul > li
5. ol > li
6. dl > dt + dd
7. table > thead + tbody > tr > th + td

+++

8. br
9. img
10. hr
11. link

+++

10. div
11. span
12. html
13. head
14. body

+++

1. article
2. section
3. aside
4. small

などなど

**これらのHTMLタグを使用して文章に意味をつけていくことをマークアップと言います**

---

### HTMLを書くために最低限の環境を整える

必要なものはテキストエディタだけ

1. メモ帳
2. 秀丸エディタ
3. **Sublime Text**
4. Atom
5. Dreamweaver

参考：[今日から使える！Sublime Textの使い方【初心者向け】](https://techacademy.jp/magazine/3060)

---

### HTMLを書いてみる

テキストエディタで新規ファイルを開く

![](https://raw.githubusercontent.com/Y-Kogawa/coding-slide/master/image001.png)

↓

+++

HTML文書の定義をする

```
<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="ie=edge">
<title>Document</title>
</head>
<body>
	
</body>
</html>
```

↓

+++

`<body></body>`の間に文字を入力する

```
<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>Document</title>
</head>
<body>

Hello World!

</body>
</html>
```

↓

+++

.htmlの拡張子で保存する

![](https://raw.githubusercontent.com/Y-Kogawa/coding-slide/master/image002.png)

↓

+++

ブラウザで保存したファイルを開く

![](https://raw.githubusercontent.com/Y-Kogawa/coding-slide/master/image003.png)


ここまでが基本的なHTMLファイルの作り方です。

---

#### 画像を表示する

```
< img src="" width="" height="" alt="" >

```

参考：[画像を表示する](http://www.tagindex.com/html5/text/img.html)

+++

#### リンクを設定する

```
<a href="" target="">リンクテキスト</a>

```

参考：[リンクを設定する](http://www.tagindex.com/html5/text/a.html)

---

### パス（path）について

1. pathとは特定のファイルを指定するための文字列のこと
2. 相対パス・絶対パス・サイトルート相対パスなどがある

+++

#### 絶対パス
```
<img src="http://hoge.com/image/photo.jpg" alt="">
```

+++

#### 相対パス
```
<img src="../../image/photo.jpg" alt="">
```

+++

#### サイトルート相対パス
```
<img src="/image/photo.jpg" alt="">
```

---

## スタイルシートの使い方

```
.class {
	margin: 0;
	padding: 10px 5px 10px;
	background-color: #f00;
}

#id {
	width: 100%;
	position: fixed;
	top: 0;
	left: 0;
}
```

参考：[CSSの基本的な書き方](https://techacademy.jp/magazine/4872)  
参考：[CSSリファレンス](http://www.tohoho-web.com/css/)  
参考：[CSS3のセレクタ全42種](http://wp-e.org/2014/05/20/2420/)

---

### スタイルシートの適用方法は３つ

+++

#### HTMLタグに直接記述する

```
<h1 style="margin: 0 0 10px; border-bottom: 5px solid #f00">見出し</h1>
```

+++

#### HTMLのhead内に記述する

```
<head>
<style type="text/css">
.class {
	margin: 0;
}
</style>
</head>
```

+++

#### CSSファイルを作成してHTMLから読み込む

```
<head>
<link href="style.css" rel="stylesheet">
</head>
```
**基本的にはこの方法を用いる**

---

