# AI_tensorflow_CNN_car
ここでは画像データからステアリングとスロットルの推論を行うCNNとDNNの練習を行う.

kerasとTensorFlow(2.5.0)を用いたFunctinalAPIを用いたニューラルネットワークを構築する.
また言語はPythonを利用している.

筆者の実行環境を以下に示します.

tensorflow:  2.9.2  
numpy:  1.24.3  
pandas:  1.5.3  
sklearn (for train_test_split):  1.2.2  
matplotlib (for pyplot):  3.7.1  
opencv (cv2):  4.8.0  
tensorflow-gpu:  True  
Python 3.8.18  


これは実際に多層のニューラルネットワークを訓練した時の経過をグラフ化したものです.
<img src="/explanation_images/01_combined_loss-checkpoint.png" 
  alt="代替テキスト"
  width="640" 
  height="480">  
縦軸は目標値との損失, 横軸epochは計算回数を示しています.




