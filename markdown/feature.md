### Feature (특징)

- 샘플을 잘 설명하는 특징

- 사람을 설명할 때, 좋은 특징:
    - Continuous: 나이, 키, 몸무게, 소득
    - Categorical: 성별, 직업, 거주지, 출신 학교/학과

- 나쁜 특징 1: (생물 분류학적) 중
    - 모두가 호머사피엔스이므로 구분할 수 없다.
- 나쁜 특징 2: 주민등록번호
    - Categorical Value로 볼 수 있음
    - 전 국민의 수 만큼 memory가 필요할 것
    - 주민등록번호만으로는 두 사람의 유사도를 알 수 없음

- 특징을 통해 우리는 특정 샘플을 수치화 할 수 있다.

### No Need of Hand-crafted Feature in Deep Learning

- Traditional Machine Learning
    - 사람이 데이터를 면밀히 분석 후, 가정을 세움
    - 가정에 따라 전처리를 하여 feature를 추출
    - 추출된 feature를 모델에 학습
    - 장점: 사람이 해석하기 쉬움
    - 단점: 사람이 미처 생각하지 못한 특징 존재 가능성

- Current Deep Learning
    - Raw 데이터에 최소한의 전처리(e.g. scale)을 수행
    - 데이터를 모델에 학습
    - 장점: 구현이 용이함, 미처 발견하지 못한 특징도 활용
    - 단점: 사람이 해석하기 어려움

### Feature Vector

- 각 특징들을 모아서 하나의 Vector로 만든 것
    - Tabular Dataset의 각 row도 이에 해당
- 각 차원(dimension)은 어떤 속성에 대한 level을 나타냄
    - 각 속성에 대한 level이 비슷할 수록, 비슷한 샘플이라고 볼 수 있음
- 우리는 feature vector를 통해 샘플 사이의 거리(유사도)를 계산 할 수 있음