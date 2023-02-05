# dacon_4Dblock
## 대회 소개
https://dacon.io/competitions/official/236046/overview/description

본 대회는 2D 이미지 내 포디블록의 10가지의 블록 패턴들의 존재 여부를 분류하는 Multi-Label Classification을 수행하는 AI 모델을 만드는 대회이다.

## 수행
train data 와 test data의 배경이 달라 이를 극복하기 위해 합성을 진행하여 train data를 여러가지로 생성하였고, test data의 배경을 train data의 배경으로 바꾸어주었다. (test data의 정보를 가져올 수 없어 train data에 test data의 배경을 입히진 못함.)
pretrained model을 사용하여 모델 설계를 하고, 최종적으로 ensemble을 하여 결과를 계산하였다.

## 파일 구조
1. image generation: 이미지 생성(합성) 코드
2. modeling: 모델 설계 코드
3. ensemble: 최종 모델들의 예측 값을 ensemble하여 계산하는 코드
