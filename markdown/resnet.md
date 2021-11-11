### Introduction

- [He et al., 2015] Deep Residual Learning for Image Recognition
- [He et al., 2016] Identity Mappings in Deep Residual Networks

### Motivations

- ImageNet 대화가 거듭될수록, 깊은 네트워크가 우승을 차지함
- 깊은 네트워크를 학습시키는데 애로 사항이 많음
    - 최적화 문제: Training loss가 잘 낮아지지 않음
- 최적의 깊이가 존재할 텐데, 깊어지면 나머지 identity 함수면 될 것 아닌가?

### Methodology

- F(x) = H(x) - x
- H(x) = F(x) + x

- Residual Block을 쌓자

### Evaluation

- 기존:
    - 레이어가 낮아질수록 낮은 성능
- Resnet:
    - 레이어가 길어질수록 높은 성능

### Later, it turns out

- Resnet은 gradient vanishing을 방지하는 방법

- 다른 gradient vanishing 방지 방법
    - Highway Networks [Srivastava et al., 2015]
    - Linear Gated Unit [Dauphin et al., 2016]

- 현재 제안되는 대부분의 큰 네트워크들은 residual connection을 차용
    - e.g. Transformer
