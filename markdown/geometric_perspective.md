### Curse of Dimensionality

- 차원이 높을수록 데이터는 희소하게 분포하게 되어 학습이 어려워진다
    - 모든 점들을 학습하기 위해서, 모든 구역들을 살펴보아야 함
    - 같은 구역 내의 점들은 서로 구별할 수 없음
- 같은 정보의 데이터를 표현할 때, 차원이 높아질수록 희소성(sparseness)이 증가
- 희소성이 높을수록 modeling의 난이도가 높아짐
    - Gaussian Mixture를 fitting하고자 할 때
    - K-means 클러스터링을 수행하고자 할 때
- 따라서 데이터의 특징(feature)을 더럽히지 않으면서 낮은 차원에서 표현해야 함

### Linear Dimension Reduction: PCA

- n차원 공간에 샘플들의 분포가 주어져 있을 때, 분포를 잘 설명하기 위한 새로운 axis를 찾아내는 과정
- 새로운 axis는 두 가지 조건을 만족해야 한다
    - 축소했을 때 나타나는 점들의 거리의 합이 최대가 되도록
    - 축소전의 점과 선의 사이 거리의 합이 최소가 되도록
- 새롭게 찾아낸 axis에 샘플들을 투사(projection)하면 차원 축소가 가능

### Why we need dimension reduction?

- Binary Classification in 2-D
- DNN can do classifie hard