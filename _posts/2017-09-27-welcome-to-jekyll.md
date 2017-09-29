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
ディレクトリの中に新しいファイル（.txtとか）を作る
![](https://cl.ly/1T1Z0X2z2V3I/Image%202017-09-29%20at%207.41.40%20PM.png)
![](https://cl.ly/442X3S1G400Y/Image%202017-09-29%20at%207.30.45%20PM.png)


## cp
```
cp
```
ディレクトリ内のファイルをコピーして新しいファイルを作る
![](https://cl.ly/161G1u2b2m1m/Image%202017-09-29%20at%207.43.27%20PM.png)

新しいディレクトリを作り、その中に別のディレクトリのファイルをコピーする
![](https://cl.ly/2Q1g2B1z102L/Image%202017-09-29%20at%207.49.59%20PM.png)
![](https://cl.ly/2o1p3t0X140Q/Image%202017-09-29%20at%208.03.26%20PM.png)

ディレクトリを中身ごと全部コピーして新しいディレクトリを作る
![](https://cl.ly/2u0r283H330v/Image%202017-09-29%20at%207.58.58%20PM.png)
![](https://cl.ly/3u0r1L0R0L1s/Image%202017-09-29%20at%208.05.11%20PM.png)











