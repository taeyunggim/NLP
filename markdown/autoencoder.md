### Overview

- Encoder와 Decoder를 통해 압축과 해제를 실행
    - Encoder는 입력(x)의 정보를 최대한 보존하도록 손실 압축을 수행
    - Decoder는 중간 결과물(z)의 정보를 입력(x)과 같아지도록 압축 해제(복원)을 수행
- 복원을 성공적으로 하기 위해, autoencoder는 특징(feature)을 추출하는 방법을 자동으로 학습

### Encoder

- 복원에 필요한 정보를 중심으로 손실 압축을 수행
    - 필요 없는 정보 (뻔한 특징)는 버릴 수도 있음  
    (e.g. 일반적인 사람의 얼굴을 학습할 때: 사람의 얼굴에서 눈은 2개이다)

### Battleneck

- 입력(x)에 비해 작은 차원으로 구성
- 따라서 정보의 선택과 압축이 발생, 차원에 따라 압축의 정도를 결정함
    - 집에 불이 나서 탈출할 때, 무엇을 들고 나갈 것인가?
- 그러므로 z는 입력(x)에 대한 feature vector라고 할 수 있다
    - 압축의 효율이 높아야 하므로, 압력에 비해 dense vector일 것

### Decoder

- 압축된 중간 결과물(z)을 바탕으로 최대한 입력(x)과 비슷하게 복원: ≈x
    - 보통 MSELoss를 통해 최적화 수행
- 뻔한 정보는 주어지지 않더라도 어차피 알 수 있기에 복원 가능

### Summary

- AutoEncoder는 압축과 해제를 반복하며 특징 추출을 자동으로 학습
    - 필요한 정보와 필요 없는 정보를 구분할 수 있게 되는 것
- Encoder로 부터 나온 중간 결과물(z)은 입력(x)에 대한 feature vector이다
    - a.k.a Embedding Vector
    - 인코더에 통과시키는 것은 feature vector에 대한 embedding 과정이라고 볼 수 있음