### Bayesian vs Frequentist

- Bayesian 관점
    - 파라미터 또한 random variable이며, prior 분포를 따를 것
    - 미래의 uncertainty까지 고려
    - prior에 대한 가정이 필요
- Frequentist 관점
    - 파라미터는 최적화의 대상
    - 현재까지의 정보를 바탕으로 추청
    - Overfitting에 취약함

### Summary

- MAP을 통해 우리는 posterior를 최대화 하는 hypothesis를 찾을 수 있음
    - 마찬가지로 주어진 데이터셋에 대한 posterior를 최대화 하는 파라미터(ø)를 찾을 수 있음
- Bayesian 관점에서는 prior에 대한 가정을 통해, 앞으로의 uncertainty까지 고려
    - 이를 통해 overfitting 등의 문제도 해결할 수 있음
- Bayesian Deep Learning에 대한 다양한 시도들도 이어지고 있음