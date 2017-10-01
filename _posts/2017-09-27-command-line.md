---
layout: post
title:  "Learn Python 3 the Hard Way: Command Line Crash Courseで学んだこと"
---

[Learn Python 3 the Hard Way](https://learnpythonthehardway.org/)の「Command Line Crash Course」で学んだことのまとめです。

## pwd

```
pwd
```
今いるdirectoryを表示

![](https://cl.ly/2W3R1O1s1U2t/Screen%20Recording%202017-09-27%20at%2003.33%20PM.gif)

## cd ~
```
cd ~
```
home directoryに戻る

![](https://cl.ly/2f2K0F0n3o0E/Image%202017-09-29%20at%2011.23.44%20AM.png)

## mkdir
```
mkdir
```
新しくdirectoryを作る

![](https://cl.ly/151b3i0v3u18/Image%202017-09-29%20at%2012.09.57%20PM.png)

![](https://cl.ly/2e1C3e430G3Y/Image%202017-09-29%20at%2012.13.12%20PM.png)

![](https://cl.ly/2H0P2I3i0p2E/Image%202017-09-29%20at%2012.10.32%20PM.png)

さらにサブディレクトリを作る時は・・・

![](https://cl.ly/1j2M1U1Q3I0m/Image%202017-09-29%20at%2012.20.00%20PM.png)

![](https://cl.ly/3E473S3L3Y3k/Image%202017-09-29%20at%2012.26.02%20PM.png)

入れ子で連続的にサブディレクトリを作る時は・・・

![](https://cl.ly/1b3l0I3C2Z2S/Image%202017-09-29%20at%207.13.49%20PM.png)

![](https://cl.ly/0y022c0n100J/Image%202017-09-29%20at%207.18.34%20PM.png)


## cd
```
cd
```
directoryを移動する

![](https://cl.ly/410Z0Q001Z3k/Image%202017-09-29%20at%205.27.59%20PM.png)

* `cd ~`＝ホームディレクトリに移動
* `cd 〇〇`＝〇〇に移動

## ls
```
ls
```
directory内のフォルダをリストアップする

![](https://cl.ly/010i17071a2v/Image%202017-09-29%20at%206.23.20%20PM.png)

![](https://cl.ly/0D3g3m2L022G/Image%202017-09-29%20at%206.31.51%20PM.png)

## rmdirまたはrm -rf
```
rmdir
```
ディレクトリを消す

![](https://cl.ly/381W0D0V2m1N/[a9c8c07fde1b3d390bb6883c123791ae]_Image%202017-09-29%20at%2011.27.42%20AM.png)

![](https://cl.ly/0f2E0K401M3h/Image%202017-09-29%20at%2011.32.50%20AM.png)

![](https://cl.ly/313r0d1Q1C1G/Image%202017-09-29%20at%2011.38.16%20AM.png)


#### *!Caution*
* 消したいディレクトリのある**１つ前の**ディレクトリに移動してから実行する

* 実行前に、消したいディレクトリの中身を空にしておく（中にさらにディレクトリがあるとエラーになる）
* 
![](https://cl.ly/042l3T1i3y0n/Image%202017-09-29%20at%2011.30.20%20AM.png)

* ディレクトリの中のファイルを全部消したい（**見えない隠しファイル**も含む）がありエラーとなる場合がある。<br>その時は**`rm -rf`**を実行する<br>
(`rm -rf ~`（＝ホームディレクトリを全消去する）は使うと危険なので使わない！)

![](https://cl.ly/1k2r2s2O0E0a/Image%202017-09-29%20at%2011.56.21%20AM.png)

![](https://cl.ly/1V35262K1h0c/Image%202017-09-29%20at%2011.53.28%20AM.png)

![](https://cl.ly/0q2i1V2w3D0K/Image%202017-09-29%20at%2012.03.51%20PM.png)

![](https://cl.ly/3D3V0g3z2P0L/Image%202017-09-29%20at%2012.04.31%20PM.png)

★"r"(recursive)：再帰的に...繰り返してコマンドを実行する<br>
★"f"(force)：強制的に...ディレクトリ消去実行時に確認されない

## pushd/popd
```
pushd
popd
```
`pushd`...現在のディレクトリを保存したまま別のディレクトリに移動する<br>
`popd`...**最後に`pushd`を実行したディレクトリに戻る**


"shori"に`pushd`で移動する

![](https://cl.ly/2n2u3d3z4038/Image%202017-09-29%20at%206.50.52%20PM.png)

→`popd`を実行すると"sexy zone"に戻る

![](https://cl.ly/1c400H2H3o3Y/Image%202017-09-29%20at%206.52.24%20PM.png)

①"kento"に`pushd`で移動する<br>
②"kento"から"fuma"に`pushd`で移動する<br>
③`popd`を実行すると**"fuma"に戻る**

![](https://cl.ly/2c29322J1S1r/Image%202017-09-29%20at%206.58.59%20PM.png)

## touch
```
touch
```
①ディレクトリの中に新しいファイル（.txtとか）を作る

![](https://cl.ly/1T1Z0X2z2V3I/Image%202017-09-29%20at%207.41.40%20PM.png)

![](https://cl.ly/442X3S1G400Y/Image%202017-09-29%20at%207.30.45%20PM.png)

②指定したディレクトリの中に新しいファイルを作る

![](https://cl.ly/2E1G0p0M1S0m/[c3c732fa0b8897a1c38f9a7769e1da8c]_Image%202017-10-01%20at%204.05.58%20PM.png)

![](https://cl.ly/0J4646423d0Q/Image%202017-10-01%20at%206.09.43%20PM.png)

## cp
```
cp
```
①ディレクトリ内のファイルをコピーして新しいファイルを作る

![](https://cl.ly/161G1u2b2m1m/Image%202017-09-29%20at%207.43.27%20PM.png)

②新しいディレクトリを作り、その中に別のディレクトリのファイルをコピーする

![](https://cl.ly/2Q1g2B1z102L/Image%202017-09-29%20at%207.49.59%20PM.png)

![](https://cl.ly/2o1p3t0X140Q/Image%202017-09-29%20at%208.03.26%20PM.png)

③ディレクトリを中身ごと全部コピーして新しいディレクトリを作る

![](https://cl.ly/2u0r283H330v/Image%202017-09-29%20at%207.58.58%20PM.png)

![](https://cl.ly/3u0r1L0R0L1s/Image%202017-09-29%20at%208.05.11%20PM.png)

## mv
```
mv
```
ファイルを移動する（ファイル名を変える）

①ファイルの名前を変える

![](https://cl.ly/0H2n0W2h063w/Image%202017-10-01%20at%203.02.19%20PM.png)

![](https://cl.ly/2L0a163w3U3w/[038519a671f0e9d1804e639e62a10105]_Image%202017-10-01%20at%2012.52.03%20PM.png)

②ディレクトリの名前を変える

![](https://cl.ly/1e0M3q0N2o05/Image%202017-10-01%20at%203.10.53%20PM.png)

③ディレクトリ内のファイルを別のディレクトリに移動する<br>
("sexy zone"内の"shori"を"~/i/love"内に移動する )

![](https://cl.ly/0V310G1G461y/[5aee8730b0e69e42315e9c5e7a8599c6]_Image%202017-10-01%20at%202.49.18%20PM.png)

![](https://cl.ly/0b3r1v0F0z0J/Image%202017-10-01%20at%202.49.34%20PM.png)

..."sexy zone"ディレクトリにいる時は・・・

![](https://cl.ly/2n043P0F3g3t/Image%202017-10-01%20at%203.25.08%20PM.png)

...ホームディレクトリにいる時は・・・

![](https://cl.ly/393p1J2V2x3y/Image%202017-10-01%20at%203.27.48%20PM.png)

![](https://cl.ly/270R2V1s131j/[5e0013747bbbe822d6250973fa20d9b5]_Image%202017-10-01%20at%202.52.51%20PM.png)


## less
```
less
```
ファイルの内容を表示する

![](https://cl.ly/2F2r0Z0S2d1z/[1db9166307961fee48fb07583e88856a]_Image%202017-10-01%20at%202.41.48%20PM.png)

![](https://cl.ly/3z2m34382h1B/Image%202017-10-01%20at%203.33.36%20PM.png)

![](https://cl.ly/2N390i300S46/[dea29bf90938553619d80374d6e1c80d]_Image%202017-10-01%20at%202.44.33%20PM.png)

* 閉じる時は"q"(＝quit)
* ↑、↓で上下にスクロール
* spacebarで一画面分下にスクロール、"w"キーで一画面分上にスクロール

![](https://cl.ly/0Y2R1e0W403G/Screen%20Recording%202017-10-01%20at%2004.23%20PM.gif)

## cat
```
cat
```
ファイルの内容を直接スクリーンに表示する

![](https://cl.ly/1y281V3m1m3c/Image%202017-10-01%20at%204.37.03%20PM.png)

## rm/rmdir
```
rm
```

①ファイルを削除する

![](https://cl.ly/3r3b0E1o1o2C/Image%202017-10-01%20at%204.41.07%20PM.png)

![](https://cl.ly/2a3V2P3s0A2c/Image%202017-10-01%20at%204.59.58%20PM.png)

![](https://cl.ly/0b3L3p1O2630/Image%202017-10-01%20at%204.41.54%20PM.png)

②ディレクトリの中のファイルを削除する

![](https://cl.ly/390v3H0w1b1z/Image%202017-10-01%20at%205.03.49%20PM.png)

![](https://cl.ly/2s0E1u1z2N3Y/Image%202017-10-01%20at%204.48.42%20PM.png)

③ディレクトリを削除する

![](https://cl.ly/352q1y3j143h/Image%202017-10-01%20at%205.13.39%20PM.png)

![](https://cl.ly/0D34271m2B2R/Image%202017-10-01%20at%204.49.43%20PM.png)


④ディレクトリの中身ごと全部削除する

![](https://cl.ly/2V1K1k2z3O3V/Image%202017-10-01%20at%204.50.41%20PM.png)

![](https://cl.ly/3c0j123H1K2G/Image%202017-10-01%20at%205.12.47%20PM.png)

![](https://cl.ly/0G1s3G1u1d26/Image%202017-10-01%20at%204.54.01%20PM.png)

## echo
```
echo
```
呼応するテキストを表示する/ファイルに書き込む

①呼応するテキストを表示する

![](https://cl.ly/0z2J2N0e1J3I/Image%202017-10-01%20at%205.46.43%20PM.png)

②呼応するテキストをファイルに**上書きして**書き込む<br>

![](https://cl.ly/0z2J2N0e1J3I/Image%202017-10-01%20at%205.46.43%20PM.png)

![](https://cl.ly/0Z1U1w0V1u0s/Image%202017-10-01%20at%205.41.15%20PM.png)

もう一度やると・・・

![](https://cl.ly/0x2Z1b2t0M2O/Image%202017-10-01%20at%205.49.14%20PM.png)

![](https://cl.ly/10312o2L2Q07/Image%202017-10-01%20at%206.01.40%20PM.png)

③呼応するテキストをファイルに**追加して**書き込む

![](https://cl.ly/1i2A3g3K070R/Image%202017-10-01%20at%205.55.08%20PM.png)

![](https://cl.ly/2B1j2i0q0M2q/Image%202017-10-01%20at%205.51.50%20PM.png)

* `>`は**上書き（全部を書き替え）**、`>>`は**追加して書き込み**

## subl

```
subl
```

現在いるディレクトリをSublime Textで開く

![](https://cl.ly/20221V240e0W/Image%202017-10-01%20at%207.13.09%20PM.png)










