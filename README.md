# TinySegmenter PHP

Taku Kudo 氏が開発した JavaScript の分かち書きライブラリ [TinySegmenter] を PHP に移植したものです。

このライブラリは、sugakenn 氏による PHP 移植版 [TinySegmenterPHP] をフォークし、Composer に対応させることで、より使いやすく改良したものです。さらに、パフォーマンスの向上や最新の PHP 機能の導入を行い、名称やクラス名の一部も改定しました。

## TinySegmenter とは？

[TinySegmenter] は、日本語の文章を単語単位で分割するシンプルな形態素解析ライブラリです。機械学習を用いたアルゴリズムを採用しており、辞書なしで動作するのが特徴です。

## 要件

- PHP 8.0 以上
- PHP の mbstring 拡張モジュールがインストールされていること

## インストール

[Composer] を使ってインストールしてください。

```bash
composer require u7aro/tinysegmenter-php
```

## 使い方

このライブラリを使用すると、日本語の文章を単語単位に分割できます。以下の例では「私の名前は中野ではありません」を分かち書きしています。

```php
use U7aro\TinySegmenter\TinySegmenter;

$text = '私の名前は中野ではありません';
$result = TinySegmenter::segment($text);

var_dump($result);
// array(10) {
//   [0]=>
//   string(3) "私"
//   [1]=>
//   string(3) "の"
//   [2]=>
//   string(6) "名前"
//   [3]=>
//   string(3) "は"
//   [4]=>
//   string(6) "中野"
//   [5]=>
//   string(3) "で"
//   [6]=>
//   string(3) "は"
//   [7]=>
//   string(6) "あり"
//   [8]=>
//   string(6) "ませ"
//   [9]=>
//   string(3) "ん"
// }
```

## 注意事項

本ライブラリはオリジナルの TinySegmenter を PHP に移植したものです。そのため、機械学習ロジック自体には変更を加えておらず、分かち書きの精度や挙動はオリジナルに準拠します。もしロジックに関するバグが発生した場合、オリジナル版の修正が行われるまで対応できない可能性がありますのでご了承ください。

## ライセンス

ライセンスはオリジナルの [TinySegmenter] および [TinySegmenterPHP] と同様に、修正BSDライセンスが適用されます。

[TinySegmenter]: http://chasen.org/~taku/software/TinySegmenter/
[TinySegmenterPHP]: https://github.com/sugakenn/TinySegmenterPHP
[Composer]: https://getcomposer.org/
