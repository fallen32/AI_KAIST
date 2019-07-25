# Bayesain Deep Learning with Monte Carlo (MC) dropout

실습 일시: 2019년 7월 22일(월), 13:30 - 17:30

담당 조교: 윤지훈 (arcprime@kaist.ac.kr), 김성엽(sungyub.kim@mli.kaist.ac.kr)

### Introduction
실습 시간에 Dropout neural network를 사용하여 모델의 uncertainty를 측정하는 방법을 배웠습니다. 다시 한 번 간략하게 설명하자면 원래 dropout의 개념은
training할 때 dropout을 켜주어서 학습을 진행할 때 ensemble 효과를 내는 것입니다 (Regularization session 때도 배우셨을 겁니다). MC dropout의
경우에는 Test phase에서도 dropout을 켜주어서 각 test point마다 $T$번의 inference를 진행하여 $T$번 나온 output을 이용하여 mean과 variance를 계산합니다.

[`assignment.ipynb`](assignment.ipynb) 파일의 세 부분만 채워주시면 됩니다.
- class MLP에서 second hidden layer 부분을 작성해주세요.
- class MLP에서 Loss function을 작성해주세요.
- train 함수 내에서 sess.run에 넘겨줄 feed_dict를 작성해주세요.

### Submission
- `assignment.ipynb` 파일 내부의 코드를 수정하고 실행한 결과를 포함하여 `assignment_<이름>.ipynb` 형태로 파일명을 바꾸어 저장 (따로 코드 실행 결과를 지워주지 않으면 실행 결과가 자동으로 함께 저장됩니다.)
- 실행해서 얻어진 그림과 자신이 기본 코드에서 추가한 부분을 기록하여 `report_<이름>.txt` 형태로 저장
- `assignment_<이름>.ipynb`, `report_<이름>.txt` 두 파일을 `submission_<이름>.zip` 으로 압축하여 제출

담당 조교 모두에게 이메일로 제출해 주시기 바랍니다.

### Grading
제출하신 결과들의 분포를 확인하고 기준을 나누어 평가할 예정입니다.
