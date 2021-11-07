### Information

- 본디, 통신이나 압축을 위해 주로 다루어지던 분야
- Representation learning에 관해서 다루다보니 자연스럽게 연결됨
- 불확실성(Uncertainty)을 나타내는 값

### Entropy

- 정보량의 기대값(평균)
- 분포의 평균적인 uncertainty를 나타내는 값
    - 분포의 형태를 예측해볼 수 있음
### Cross Entropy

- 분포 P의 관점에서 본 분포 Q의 정보량의 평균
- 두 분포가 비슷할 수록 작은 값을 가진다

### KL-Divergence and Cross Entropy

- KL-Divergence와 Cross Entropy를 ø로 미분하면 같다

### Summary

- Objective:
    - 확률 분포 P(x)로부터 수집한 데이터셋 D를 통해, 확률 분포 함수 P(y|x)를 근사하고 싶다.
- 확률 분포 함수 신경망 Pø(y|x)를 통해 이를 수행하자
- KL-Divergence(또는 Cross Entropy)가 최소가 되도록 gradient descent 수행