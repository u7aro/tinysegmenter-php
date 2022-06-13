# TinySegmenterPHP
TinySegmenter:Javascriptだけで書かれたコンパクトな分かち書きソフトウェア (c) 2008 Taku Kudo のPHP移植版です

>TinySegmenterはフリーソフトウェアです. 修正BSDライセンスに従って本ソフトウェアを使用,再配布することができます.

TinySegmenterPHPも同様です。

# 使い方
$segmenter = new TinySegmenterPHP();

$segs = $segmenter->segment("私の名前は中野ではありません"); 

var_dump($segs);

