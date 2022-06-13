# TinySegmenterPHP
TinySegmenter:Javascriptだけで書かれたコンパクトな分かち書きソフトウェア (c) 2008 Taku Kudo のPHP移植版です

>TinySegmenterはフリーソフトウェアです. 修正BSDライセンスに従って本ソフトウェアを使用,再配布することができます.

TinySegmenterPHPも同様です。

[本家TinySegmenterの説明やソースコードはこちらです](http://chasen.org/~taku/software/TinySegmenter/)
## 使い方
$segmenter = new TinySegmenterPHP();

$segs = $segmenter->segment("私の名前は中野ではありません"); 

var_dump($segs);

## お断り
自分がTinySegmenterをPHPで使いたかったので、JavaScriptのコードをPHPに変換しただけです。

たぶんコードの前半が機械学習の学習データなんだろうな、ぐらいにしかわかりません。

コード中のコメントアウト部
//$score += $this->ts_(TinySegmenterPHP::$TC5__,$c4 . $c5 . $c6);
は本家のコードからそのまま踏襲しています。

