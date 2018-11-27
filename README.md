# LDPCの勉強用

## はじめに

python使ってLDPCのデコーダを実装するまでやってみようと思う。


## 01_hamming_encoding.py

ハミング符号のエンコーディング。

- [ハミング符号 - Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%8F%E3%83%9F%E3%83%B3%E3%82%B0%E7%AC%A6%E5%8F%B7)

- `n`: 符号長。最終的に出力されるビット数。
- `k`: 情報数。入力されるビット数。
- `m`: 冗長化ビット数。m = n - k
- `H`: 検査行列。m×n、つまり7×3の行列。AとI_mから作られる。
- `A`: 検査行列の前半。
- `I_m`: m×mの単位行列。単位行列は対角だけ1になってるやつ。
- `G`: 生成行列。[I_k A^T]で作る。
- `y`: 符号化ビット列。ハミング符号をかけた後の出力ビット列。nビット。
- `x`: 入力ビット列。入力データ。kビット。

4bitの入力に対して7bitのデータを出力するハミング符号を(7, 4)ハミング符号と言う。




## 参考リンク

- [ハミング符号 - Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%8F%E3%83%9F%E3%83%B3%E3%82%B0%E7%AC%A6%E5%8F%B7)
- [誤り訂正符号の実例](http://www2.math.kindai.ac.jp/~chinen/err_corr_f/err_corr.html)
