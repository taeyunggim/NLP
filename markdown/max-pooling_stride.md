### Dimension Reduction

- 고차원 공간의 sparse한 데이터에 저차원 공간에 mapping
    - 그 과정에서 복잡하게 얽혀 있는(entangle) 데이터를 풀어냄
- 하지만, '3x3 + 1 padding' conv layer는 입출력 텐서의 크기가 같음

### Max-pooling
- Down sampling 기법

### Stride
- Working in convolution layer

### Dimension Reductions in CNN
- Max-pooling
    - 별도의 max-pooling layer를 활용
    - 초기에 많이 활용됨
- Stride
    - 같은 conv layer 내에서 간단히 동작
    - 근래에 좀 더 애용되는 추세