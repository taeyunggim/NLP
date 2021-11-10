### Summary

- 예전부터 영상 처리 분야에서는 Convolution Filter를 활용
    - 탐지하고자하는 패턴에 따라 필터를 손으로 하나하나 깎아 구성
- CNN은 데이터셋의 x와 y의 구성에 따라 자동으로 탐지해야 할 패턴을 추출
    - 따라서 내부 kernel은 해당 패턴을 추출하기 위한 형태로 자동으로 구성됨
- FC Layer에 비해 매우 빠르고 적은 weight parameter를 가짐

### 사용 예시

- Text classification(2014)
- Machine Translation(word2vec)
- Time series(주가 예측)

### 실전 꿀팁

- CNN의 특징
    - FC Layer에 비해 입출력 크기가 계산이 까다로워, 네트워크 구성이 쉽지 않다.
- how to design CNN Architecture
    - CNN Block
        - 1) 3x3 Convolution Layer
        - 2) ReLU
        - 3) Batch Normalization
        - 4) 3x3 Convolution Layer (+ with Stride size (2x2))
        - 5) ReLU
        - 6) Batch Normalization
        - 7) (+ Max-pooling if no stride)

### Exercise Briefing

- Enhanced MNIST Classification using CNN
    - Upgrade the classifier from FCNN to CNN

### Before Deep Learning

- Convolution filter를 활용하여 hand-crafted feature 추출

### In Deep Learning

- x -> y 의 관계의 학습에서 필요한 feature를 추출하기 위한 convolution filter를 자동 학습

### vs Fully-connected Layer

- 매우 빨르고 작은 weight parameter를 가짐
- 입출력 크기가 계산이 까다로워, 네트워크 구성이 쉽지 않다
    - 3x3 커널을 활용하면 그래도 좀 낫다

### Warm-up

- Computer vision 분야에서 CNN을 뗄 수 없는 존재
- 패턴 인식에서 워낙 월등함을 보여주므로, NLP 등의 다른 분야에도 활발히 사용됨