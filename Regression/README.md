### Machine Learning?
### 특징이 추출된 입력을 특정 알고리즘(수식)을 학습해서 결과를 예측하는 방법<br><br>ex)사람의 다양한 정보중 키를 입력해서 몸무게를 예측하는 1차함수 수식 설계 및 학습
### Linear Regression?
### 연속된 숫자 중 실제 값과 유사한 값을 예측
### 결과를 가장 잘 예측하는 직선을 찾는 알고리즘
### y = ax + b 와 같은 1차 함수를 사용
### 학습 데이터에서 *x와 y간의 pattern을 학습해서 최적의 a,b를 찾는것*
### 최적의 learnable parameters를 찾기 위해 예측값 - 실제값인 error를 구하고 오차 제곱의 합 평균이 작을수록 좋은 MSE(Mean Square Error)를 사용해서 평가
### Method of Least Squares
### Multiple Regression: 입력하려는 feature가 1개가 아닌경우에는 1차함수를 통해 수식을 나타낼 수 없음
### Polynomial Regression:1차함수가 아닌 곡선형태를 나타낼 수 없음
### *따라서 Linear Regression으로는 해결할 수 없는 많은 parameter의 처리를 위해 다른 방법이 필요*
### MSE 최소화: 모든 learnable parameter에 대해 모든 경의 수의 MSE를 연산해서 탐색
### Cost가 너무 높음 > Gradient Descent(경사 하강법): 기울기를 통해 최저점을 찾아나감
### y = a*W(편의상의 표현) + b의 그래프를 미분해서 극소값을 가지는 leanable parameter 쌍을 찾는 것이 목표
### 이때, 극소값을 찾기 위해 한 번 이동하는 거리 alpha를 learning rate라고 부름
### Logistic Regression
### Linear Regression은 연속적인 수를 가지는 결과를 예측하기 위해 사용
### 따라서 0/1 분류와 같은 classification은 할 수 없음
### Logistic Regression: 1차함수의 모양이 아닌 데이터의 모형과 비슷한 모양을 가지는 함수를 채택
### Threshold를 통해 0/1로 분류도 가능<br>*Sigmoid*라는 함수를 사용해서 그래프를 나타냄
### Cross entropy loss: 기존 regression과 다르게 해당 class를 맞췄냐에 따른 cost function 사용
### Cost function이 0에 가까워지면 더 많은 정답을 맞췄음을 의미(아래의 수식 참조)
![Screenshot-2020-10-15-at-3 13 11-PM](https://github.com/YongwanJoo/Deep-Learning-study/assets/113014598/c81f6fd0-a2e6-4a44-b193-cc0e81f1fa8e)
