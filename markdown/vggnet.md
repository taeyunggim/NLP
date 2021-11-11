### Introduction

- [Simonyan et al., 2014] VERY DEEP CONVOLUTIONAL NETWORKS FOR LARGE-SCALE IMAGE RECOGNITION
- 2014년 ImageNet 대회에서 2등 (GoogleNet이 1등)
    - 2등에도 불구하고 편리하고 가벼운 사용성으로 인해 인기
- VGG16, VGG19와 같이 다양한 버전이 존재

### Motivations

- 기존 네트워크들은 5x5 또는 7x7 conv, layer를 사용
    - layer를 거칠 때마다, feature map의 축소 발생
- 3x3 conv, layer를 반복 사용하여 5x5 또는 7x7 conv.layer를 대체 가능
    - 3x3 2번 -> 5x5 conv.layer
    - 3x3 3번 -> 7x7 conv.layer
- +1 padding을 활용하면 feature map의 크기 유지 가능
- 결과적으로 더 깊은 네트워크 달성 가능
    - 더 적은 weight로 더 큰 capacity를 달성

### Methodology

- 1) 3x3 conv.layer + 1 padding
- 2) 활성 함수 + BatchNormaliztion
- 3) 필요에 따라 1~2번 반복
- 4) 2x2 maxpooling

- maxpooling은 stride로 대체 가능
- 더 깊지만 더 작은 파라미터를 가진 네트워크

### Summary

- 가볍고, 편리하여 많은 분야에 다양하게 활용됨
    - e.g. object detection, image segmentation
- 마지막의 FC layer는 단점으로 지적됨