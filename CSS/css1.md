# CSS Handson

## CSS とは？

CSS は HTML にスタイル機能を提供する言語です  
HTML がページのコンテンツを記述するための言語なのに対し、CSS はそのコンテンツの表示の仕方をコントロールするもの  
つまり、デザインするやつ！！！！

## CSS を書く場所

index.html

```
<p style="color: yellow;">ねこ</p>
```

ねこが赤くなる

```
<p>ぞう</p>
<style>
  p{color: blue;}
</style>
```

ぞうが青くなる  
など書ける

**body の中に書きましょう！**

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
  <p>ぞう</p>
  <style>
    p{color: blue;}
  </style>
</body>
</html>

```

### 基本は外部ファイルで書く

css ファイルをつくる
style.css を html と同じ場所につくろう！  
-index.html  
-style.css

拡張子は.css

style.css

```
p {
color: #ff0000;
}
```

このようにカラーコードでも指定できる

css の外部ファイルを読み込もう！  
head に書こう！

index.html

```
<link rel="stylesheet" href="style.css">　
```

すべて書くとこんな感じ。

index.html

```
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>サイトタイトル</title>
  <meta name="description" content="サイトの説明を記載します">
  <link rel="icon" href="favicon.ico">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- ここにコンテンツを記載します -->
  <p>ぞう</p>
  <p>ねこ</p>
</body>
</html>
```

style.css

```
p {
color: #ff0000;
}
```

ねことぞうの色がかわることを確認する

## CSS のクラス属性

HTML のタグに CSS のクラスを当てることでデザインを加えることができます。  
しかし、結構ややこしいので、実際にやりながら見てみましょう！

**class 属性を追加する**

class 属性の書式

```
divタグの場合
<div class="クラス名"></div>をつける

pタグの場合
<p class="クラス名">帰納法</p>
```

実際に書いてみよう!

index.html

```
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>サイトタイトル</title>
  <meta name="description" content="サイトの説明を記載します">
  <link rel="icon" href="favicon.ico">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- ここにコンテンツを記載します -->
  <p class="elephant">ぞう</p>
  <p class="cat">ねこ</p>
</body>
</html>
```

style.css

```
.elephant{
  color: yellow;
}
.cat{
  color: red;
}

```

class 属性は、そのタグが所属するグループの名前を指します。

`class`を用いることで、タグを指定して style を適用することができます。

[最初に戻る](https://github.com/cistLT-Club/HTML_CSS_JavaScript_Handson_2021)
