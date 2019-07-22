# 삼성 DS-KAIST AI Expert 프로그램 
## Week 3. CNN과 RNN

실습 일시: 2019년 7월 17/18일 (수, 목)

담당 조교: 이세현 (cogito288@gmail.com)

### Introduction
이번 과제는 CNN 과 RNN 에서 각각 1문제씩 제출되었습니다.

1. CNN : CNN에서의 간단한 convolution 연산과 pooling 연산을 직접 계산해보며 CNN의 특징추출 단계를 이해하기 위한 과제입니다. 과제에 대한 자세한 설명은 CNN 폴더의 `CNN_과제설명.pdf` 파일을 참고 부탁드립니다.

2. RNN : 교수님이 수업에서 다루셨던 Turing Recurrent Network [Hyotyniemi 1996]에 관한 숙제입니다. 교수님의 강의 자료와 추가 제공되는 PPT를 참고부탁드립니다. 예시 코드는<code>example.ipynb</code>를 참고 부탁드립니다. 
- 1. V0 <- V0
- 2. V1 <- V1-1
- 3. V0 <- V0+1
- 4. IF V1 $ \neq $ 0 GOTO 6
<a href="https://www.codecogs.com/eqnedit.php?latex=\neq" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\neq" title="\neq" /></a>
- 5. V0 <- V0+1
- 6. V1 <- V1-1
- 7. END (Do Nothing)

- 다음 instrunctions에 해당하는 transition matrix를 찾아제출하고, initial state가 V0=1, V1=2일 때 instruction 1부터 실행하여 얻게되는 steady state 결과를 제출하시면 됩니다. 또한 initial state가 V0=1, V1=1일 때 instrunction 1부터 실행하여 얻게 되는 steady state결과도 보고서에 적어주십시오. 보고서에서는 transition matrix를 적어주시고, 각 initaial state마다 instrunction을 거치며 steady state까지 가는 중간 state을 적어주시면 됩니다. 과정의 경우, 손으로 계산하셔도 되고 프로그래을 짜서 하셔도 됩니다.


### Grading

1. CNN :
- (1)번 문제의 matrix : 2점
- (2)번 문제 객관식 : 1점
- (3)번 문제의 matrix : 2점

2. RNN : 
- 보고서: 2.5점
- transition matrix 정답: 1.5점
- initial state의 steady state 정답: 1점

총 10점

### Submission

#### 1. CNN :
-  `CNN` 폴더를 생성해주세요.
- (1),(2),(3) 에 대한 정답을 하나의 파일 `CNNreport_이름.pdf` 에 저장해주세요.

#### 2. RNN : 
- `RNN` 폴더를 생성해주세요.
- 과제 진행 과정에서 수정한 코드에 대한 간략한 보고서를 `RNNreport_이름.pdf` 저장해주세요.
- 프로그램을 이용하여 푸신 경우 코드는 `RNNcode_이름.ipynb`로 저장해주세요.


#### 최종 제출 파일 : `Assignment_0718_이름.zip`
- `CNN` 폴더와 `RNN` 폴더를 압축하여 보고서와 필요에 따라 코드가 포함된 하나의 zip 파일 `Assignment_0718_이름.zip`을 조교 메일을 통해 제출해주시면 됩니다.

