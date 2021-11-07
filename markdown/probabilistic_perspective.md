### About

- Neural Networks는 확률 분포 함수를 모델링 할 수 있음
    - 이를 통해 가상의 확률 분포 함수 P(y|x)를 근사(approximation)할 것
- 대부분의 최신 기술들은 이 관점에 기반을 두고 만들어짐
- DNN 확률 분포로 보았을 때, 가능한 이론들
    - Likelihood
    - Maximum Likelihood Estimation (MLE)
    - Maximum A Posterior (MAP) Estimation
    - Cross Entropy & KL-Divergence

### Basic
- Random Variable & Probability Distribution(어떤 변수 x가 x라는 값을 가질 확률)
- Discrete Probability Distribution(확률의 총 값은 1)
- Continuous Probability Distribution(확률 밀도)
- Conditional Probability(조건부 확률 분포)
- Bayes Theorem(데이터 D가 주어졌을 때, 가설 h의 확률)
- Exception and Sampling(수식)
- Monte-Carlro(확률 분포로부터 샘플링을 통해 함수의 가중 평균 구하기)

### After

- Our objective is:
    - 우리의 세계(머릿속)에 존재하는 가상의 확률 분포 함수를 모사하자
- 확률 분포 P(x)에서 수집한 입력 데이터 x에 대해서 원하는 조건부 확률 분포 P(y|x) 또는 샘플링한 출력 데이터 y를 반환하도록, 손실함수를 최소화하는 확률 분포 함수의 파라미터(ø)를 찾자
    - Maximum Likelihodd Estimation
- Gradient descent를 수행하기 위해 back-propagation을 수행하자