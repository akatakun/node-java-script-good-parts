---
datetime: 2016-11-01 20:07:01
layout: mou
title: JavaScript The Good Parts
thumb:
---
## 良いパーツ
* 関数
* 緩い型付け
* 動的なオブジェクト
* 強力なオブジェクトリテラル記法(JSONと同様のフォーマット)


## 悪いパーツ
* グローバル変数に依存したプログラミングモデル


## 命令文
JavaScriptはコンパイルユニットをすべて1つの一般的なグローバルな名前空間に投げ込んでしまう

JavaScriptのブロックは新しいスコープを作成しない


## オブジェクト
数値，文字列，真偽値はイミュータブル  
オブジェクトはミュータブル  
ともにメソッドが呼び出しができる

配列，関数，正規表現もオブジェクト  
オブジェクトは参照渡し


## プロパティ
キーは文字列で変数名の規則(文字列から始まり数値，文字列，アンダースコアで構成される)に沿っていればクォートは省略できる  
値はundefined以外

メンバには[]ないしは変数名の規則に沿っていれば.でアクセスできる  
存在しないメンバにアクセスするとundefinedが返る


## プロトタイプ
すべてのオブジェクトはプロトタイプオブジェクト(Object.prototype)とリンクしており、そこからプロパティを引き継いでいる  
プロトタイプオブジェクトにプロパティが追加された瞬間、すべての個オブジェクトからプロパティにアクセスできるようになる

```js
if (typeof Object.create !== 'function') {
  Object.create = function(o) {
    var F = function() {};
    F.prototype = o;
    return new F();
  }
}
var another_stooge = Object.create(stooge);
```





## 参考
[![alt text](https://jp.searchpreview.de/preview?s=)]()
[]()


# node-java-script-good-parts
