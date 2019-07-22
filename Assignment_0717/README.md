# Deep learning regularization and optimization

실습 일시: 2019년 7월 17일(수), 9:00 - 13:00

담당 조교: 이준영 (joonyoung.yi@kaist.ac.kr), 백용수(yongsubaek@mli.kaist.ac.kr)

### Introduction
지금까지 배운 regularization, optimization 기법들을 이용하여 가장 높은 성능을 끌어내는 과제입니다.

[`assignment.ipynb`](assignment.ipynb) 파일을 잘 읽으시고 지시하는 과제를 수행하시기 바랍니다.

!**주의**하실 점은 주어진 모델의 형태를 수정해서는 안됩니다. 

기본 모델: \[(Input: 32*32) -> 512 -> 512 -> 512 -> (Output: 10)\] 

Dropout 등의 layer는 추가하실 수 있지만 기본 모델의 hidden layer, unit 수는 변경하실 수 없습니다.

### Submission
- `assignment.ipynb` 파일 내부의 코드를 수정하고 실행한 결과를 포함하여 `assignment_<이름>.ipynb` 형태로 파일명을 바꾸어 저장 (따로 코드 실행 결과를 지워주지 않으면 실행 결과가 자동으로 함께 저장됩니다.)
- 실행해서 얻어진 최종 성능(final_test_accuracy)과 자신이 기본 모델에서 수정한 regularization, optimization 기법을 간단히 기록하여 `report_<이름>.txt` 형태로 저장
- `assignment_<이름>.ipynb`, `report_<이름>.txt` 두 파일을 `submission_<이름>.zip` 으로 압축하여 제출

담당 조교 모두에게 이메일로 제출해 주시기 바랍니다.

### Grading
제출하신 결과들의 분포를 확인하고 기준을 나누어 평가할 예정입니다.
