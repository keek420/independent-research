
自主研究で行ったデータやコード等

# CycleGANを用いた雪景色変換
## 概要
CycleGANは、2つの異なるドメイン間の画像変換を実現する深層学習モデルです。本記事では、CycleGANを用いて、雪景色と非雪景色の画像変換を行います。

## 環境構築
本記事では、Python 3.7以上とtensorflow 1.5以上が必要です。また、GPUを使用する場合はCUDAが必要です。

## データセット
本記事では、tensorflow datasetを使用します。

## モデル
CycleGANは、2つのジェネレーターと2つのディスクリミネーターで構成されます。ジェネレーターは、入力画像をターゲット画像に変換することを目的としています。ディスクリミネーターは、入力画像が本物の画像であるか、生成された画像であるかを判断することを目的としています。CycleGANは、2つのジェネレーターと2つのディスクリミネーターを使用して、2つのドメイン間の画像変換を実現します。
