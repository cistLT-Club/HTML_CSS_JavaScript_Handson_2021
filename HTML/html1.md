# HTML Handson

## 0. HTML とは？

HTML とはハイパーテキストマークアップランゲージの略で、Web ページを作成するために開発された言語です。  
タグを利用して、見出しや段落、表といった要素を書き並べていくことができます。  
今回は HTML の基本的な構造と書き方、最低限覚えておくといいタグを紹介します！！

## 1. HTML の雛形

HTML の形はこれだ！

```
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>サイトタイトル</title>
  <meta name="description" content="サイトの説明を記載します">
  <link rel="icon" href="favicon.ico">
</head>
<body>
  <!-- ここにコンテンツを記載します -->
</body>
</html>
```

これをまずは覚えよう！！  
困ったらこれをコピペしよね。  
(VScode の場合は'!'で補間されます。)

## 2. 覚えておくべきタグ

### h1, h2, h3, etc...

見出しには`<h1>`〜`<h6>`タグを使います。  
`<h1>1番目に大きな見出し</h1>`  
`<h2>2番目に大きな見出し</h2>`  
`<h3>3番目に大きな見出し</h3>`  
...  
というように使います。

```
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>タイトル</title>
  <meta name="description" content="サイトの説明を記載します">
  <link rel="icon" href="favicon.ico">
</head>
<body>
  <!-- ここにコンテンツを記載します -->
  <h1>1番目に大きな見出し</h1>
</body>
</html>
```

上記のように`<body></body>`の中に表示したいものを書きます。

### p

`<p>`タグは文章の段落を表すときに使います。  
`<p>春はあけぼの。</p>`  
`<p>夏は、夜。</p>`

### br

`<br>`で改行します。

### img, image

画像には`<img>`タグを使います。単独で使って、「どの画像を表示したいか」を src 属性で指定します。  
`<img src="画像名.jpg" alt="説明">`

`src`には画像の**パス**を指定します。

相対パス、絶対パスのいずれかで指定します。

[相対パス　絶対パスの違い](https://techacademy.jp/magazine/5801)

### a

リンクを貼るには`<a>`タグを使いましょう。  
`<a href="https://cist-lt-group.web.app/">CistLT</a>`  
というように、リンクさせたい部分をタグではさみます。

### div

`<div>`〜`</div>`で囲んだ部分をひとまとまりにし、スタイルシートを適用させたいときなどに使います。

```
<div>
 <p>春は、あけぼの。</p>
 <p>夏は、夜。</p>
</div>
```

### span

`<span>`〜`</span>`も囲んだ部分をひとまとまりにし、スタイルシートを適用させたいときなどに使います。  
div との違いとして、`<div>` はブロック要素(前後に改行がはいる)、` <span>` はインライン要素(前後に改行が入らない)という違いがあります。

例

`<p>cist<span>LT</span></p>`

```
<div>
 <p>春は、あけぼの。</p>
 <p>夏は、夜。</p>
</div>
```

### ol, ul, li

`<ol>`,`<ul>`,`<li>`タグはリストを表します。  
`<ol>`…番号付きの箇条書き  
`<ul>`…番号のない箇条書き  
`<li>`…リストの項目を記述

例

```
<ol>
  <li>リスト１</li>
  <li>リスト２</li>
</ol>
```

```
<ul>
  <li>リスト１</li>
  <li>リスト２</li>
</ul>
```

### table td th

`<table>` テーブル(表)をつくる  
`<td>`タグは、表のデータセルを作成する際に使います  
`<th>` テーブル（表）の見出しセルを作成する

[表の作り方](https://www.sejuku.net/blog/49377)

[CSS Handson へ進む](https://github.com/CIST-LT-CLUB/HTML_CSS_JavaScript_Handson_2021/blob/master/CSS/css1.md)  
[最初に戻る](https://github.com/CIST-LT-CLUB/HTML_CSS_JavaScript_Handson_2021/blob/master/README.md)
