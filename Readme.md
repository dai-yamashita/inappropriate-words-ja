# 概要
チャットボットやSNS、もしくはそれらのデータを用いての解析において、不適切表現のフィルタリングをするための不適切表現単語リストです。

utf-16も考えましたが、現状絵文字のたぐいの殆どがutf-8内に収まっていると考えたのでutf-8です。

# ファイル

## Sexual.txt
性的な表現のリストです。内部はソートされてます。

## word_inserter.py
単語を追加するときに使っているプログラムです。

wort_inserter.py [filename] [-w [words1 words2...]] [-s [souce_file]]

です。filenameは必須で新たな単語を挿入する先のファイル名(e.g. Sexual.txt)を指定します

-w はコマンドラインに入力した単語を追加できます。スペース区切りで複数いけます。  
-s はSexual.txtと同様に改行で区切られた単語ファイルからimportするときに使います。  
**ちょっとサボったので同一ディレクトリのファイルからしか今はインポートできません。**
