# 삼성 DS-KAIST AI Expert 프로그램 
## Week 3. Autoencoder, VAE, GAN 과제

실습 일시: 2019년 7월 19일 (금), 13:30 - 17:30

담당 조교: 박종진 (pjj4288@kaist.ac.kr)

### Introduction

첨부된 `assignment.ipynb` 파일의 주석으로 표시된 미구현 부분을 완성하고 그 결과를 확인해주세요. 실습시간 코드의 답안지를 못 받으신 분들을 위해 `gan_vae_sol.ipynb` 파일도 첨부합니다.

본 과제에서는 실습시간 Part 2에서 다룬 GAN을 활용하여 운동화나 셔츠 같은 옷 이미지를 생성하는 모델을 만들어볼 것입니다. 여러가지 GAN 모델 중, class-conditioning이 가능한 모델인 ACGAN을 학습할 것입니다. 10개의 클래스와 70,000개의 흑백 이미지로 구성된 Fashion-MNIST 데이터셋을 사용하여 학습한 뒤 그 결과를 확인합니다.

### Submission

`assignment.ipynb` 파일 내부의 코드를 수정하는 방식으로 과제를 진행한 뒤, 생성된 이미지와 코드가 포함된 `Assignment_0719` 폴더의 이름을 `Assignment_0719_이름` 형태로 바꾸어주시고 zip파일 형태로 압축해주세요. 즉 제출파일 이름은 `Assignment_0719_이름.zip`이 되는데, 이를 조교 메일을 통해 제출해주시면 됩니다.