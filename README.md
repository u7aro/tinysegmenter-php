# TinySegmenterPHP
TinySegmenter:Javascriptだけで書かれたコンパクトな分かち書きソフトウェア (c) 2008 Taku Kudo のPHP移植版です

>TinySegmenterはフリーソフトウェアです. 修正BSDライセンスに従って本ソフトウェアを使用,再配布することができます.

TinySegmenterPHPも同様です。

[本家TinySegmenterの説明やソースコードはこちらです](http://chasen.org/~taku/software/TinySegmenter/)
# 使い方
$segmenter = new TinySegmenterPHP();

$segs = $segmenter->segment("私の名前は中野ではありません"); 

var_dump($segs);

# お詫び
自分がPHPで使いたかったので、JavaScriptのコードをPHPに変換しただけで、詳しいことはよくわかりません。

たぶん、コードの前半が機械学習の学習データだということは予想がつきます。

コード中のコメントアウト部は、本家のコードから踏襲しています。

