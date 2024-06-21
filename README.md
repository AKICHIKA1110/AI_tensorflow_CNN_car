# カメラで衝突回避を行う深層学習モデル

このプロジェクトでは, 単眼カメラから取得した画像データを用いて衝突回避を行う深層学習モデルを構築した.
![俯瞰動画](./explanation_images/Bird's-eye-view.gif)

## プロジェクトの概要

単眼カメラのみで周囲の環境を認識し, 障害物を検知して回避することを目的としています.本プロジェクトでは, 以下のステップを踏んでモデルを構築します.

1. データ収集：単眼カメラを用いて障害物が存在する環境の画像データを収集します.
2. データ前処理：収集した画像データを前処理し, モデルの入力として適した形式に変換します.
3. モデル構築：深層学習モデルを構築します.
4. モデル学習：前処理したデータを用いてモデルを学習させます.
5. モデル評価：学習したモデルの性能を評価します.

## ファイルの説明
- `cnn_model.ipynb`:モデル構築, ネットワークモデルの学習, 学習推移の可視化を含んでいる
- `kogakuin_model.ipynb`:モデルの読み込みを行う実行ファイル
- `kogakuin_model.h5`:ネットワークの構造とパラメータを含んだ学習済みモデルのファイル

## 詳細
dataセットとなるファイルは4つ存在する.   
`1_image_data`:  
`2_image_data`:  
`3_image_data`:  
`4_image_data`:  
この4つファイルの中に存在する`list2.txt`ファイルには正解ラベルと画像データの名前が保存されている.

## ライブラリの依存関係
### 学習を行うためのノード(Windows, Google colabo)
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
### Raspberry Pi 3 Model B+
- TensorFlow
- Keras
- OpenCV
- Numpy

これらのライブラリは, 以下のコマンドでインストールできます.

```sh
pip install tensorflow keras opencv-python numpy matplotlib
```
