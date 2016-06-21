# Parallax.jsの使い方

下記のjQueryプラグインの簡潔な使い方です。

- http://pixelcog.github.io/parallax.js/

## デモ
- http://sutara79.github.io/demo-parallax.js/01.html

## 注意: IEやEdgeで画面がチラつく場合がある
`<body>`と`<html>`には、`position: static`以外を指定してはなりません。  
InternetExplorerやEdgeで**マウスホイールを使って**画面をスクロールさせると、画面がチラつきます。  
下記のページをIEまたはEdgeで開いてみてください。

- http://sutara79.github.io/demo-parallax.js/02.html

なお、`<body>`と`<html>`以外の親要素の`position`は影響しません。

- http://sutara79.github.io/demo-parallax.js/03.html

このことから、フッターを常に画面下部に固定するための、下記のようなCSSテクニックとの併用ができなくなります。  

- 参考: [[CSS]フッタの表示をコンテンツ量が少ない時は最下部に固定、多い時は成り行きにするシンプルなテクニック | コリス](http://coliss.com/articles/build-websites/operation/css/css-simple-sticky-footer-by-melissa.html)

上のテクニックでは、`<html>`に`position: relative;`を指定しています。  
他の似たようなテクニックでも`<body>`と`<html>`のどちらかを`relative`にしています。

ただ、視差効果を狙ったページは総じて縦長であり、画面の高さ以上の長さになることはほぼ間違いないので、問題ないと思います。

## 注意: jQuery3.0では動作しない
2016年6月現在、parallax.jsの最新バージョンは1.4.2ですが、jQuery3.0.0では動作しないようです。

- http://sutara79.github.io/demo-parallax.js/04.html
