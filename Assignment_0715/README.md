# 삼성 DS-KAIST AI Expert 프로그램 
## Week 3. 신경망 기초, 다층신경망: 프로그래밍 과제

실습 일시: 2019년 7월 15일 (월), 13:30 - 17:30

담당 조교: 정종헌 (jongheonj@kaist.ac.kr)

### Introduction

지난 실습 중에서는 TensorFlow를 사용하여 2-layer LSTM 모델을 구성하고, 해당 모델을 사용해 색의 이름으로 
해당 색을 예측하는 ColorBot을 학습하는 다루는 내용이 있었습니다. 해당 모델은 잘 동작하지만, 
모델을 빌드하는 과정에서 아래와 같은 경고문이 등장하는 것을 확인할 수 있습니다:
```
WARNING: Logging before flag parsing goes to stderr.
W0714 22:57:01.169573 140003455665920 lazy_loader.py:50] 
The TensorFlow contrib module will not be included in TensorFlow 2.0.
...
W0714 22:57:01.174833 140003455665920 deprecation.py:323] From <ipython-input-3-4cd5c35f31ea>:16: BasicLSTMCell.__init__ (from tensorflow.python.ops.rnn_cell_impl) is deprecated and will be removed in a future version.
Instructions for updating:
This class is equivalent as tf.keras.layers.LSTMCell, and will be replaced by that in Tensorflow 2.0.
```
```
W0714 22:57:01.178820 140003455665920 rnn_cell_impl.py:702] <tensorflow.python.ops.rnn_cell_impl.BasicLSTMCell object at 0x7f5398155438>: Note that this cell is not optimized for performance. Please use tf.contrib.cudnn_rnn.CudnnLSTM for better performance on GPU.
W0714 22:57:01.181288 140003455665920 rnn_cell_impl.py:702] <tensorflow.python.ops.rnn_cell_impl.BasicLSTMCell object at 0x7f5410545940>: Note that this cell is not optimized for performance. Please use tf.contrib.cudnn_rnn.CudnnLSTM for better performance on GPU.
```

해당 경고문은 현재 버전의 코드가 가진 두가지 문제점을 알려줍니다:
1. 현재 실습 실험환경인 TensorFlow 1.14.0 버전에서는 본 코드가 동작하지만, TensorFlow 2.0 부터는 잘 동작하지 않을 것입니다.
2. 현재 모델에서 사용되고 있는 `BasicLSTMCell`은 성능에 최적화되지 않아서 느릴 수 있습니다.

본 과제에서는 실습때 다룬 해당 코드를 업데이트하여, TensorFlow 2.0에서도 문제없이 사용할 수 있고 (가능하다면) 성능도 개선시키는 것이 목표입니다. 

### Submission

`assignment.ipynb` 파일 내부의 코드를 수정하는 방식으로 과제를 진행한 뒤, 
`assignment_<이름>.ipynb` 형태로 파일명을 바꾸어 조교 메일을 통해 제출해주시면 됩니다.
