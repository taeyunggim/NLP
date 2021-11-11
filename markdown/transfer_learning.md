### Feature Extraction in each Layer

- 각 conv.layer는 위취에 따라, low-level 또는 high-level feature를 추출하도록 학습됨
- 따라서 ImageNet의 데이터를 통해 학습된 네트워크(e.g. VGGNet)는 해당 task를 수행하기 위한 feature extraction 능력이 있을 것

### Motivations

- 데이터가 다르더라도 이미지를 활용한 task에서는 공통된 feature들이 존재할 것

### Transfer Learning이란?

- Transfer learning is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a diffrent but related problem
- How to
    - 1) Set seed weights and train as normal
    - 2) Fix loaded weights and train unloaded parts
    - 3) Train with different learning rate on each part

### Summary

- 큰 데이터셋을 통해 미리 훈련한 네트워크를 나의 문제에 재학습 시키자
    - 인터넷에 공개되어 있는 많은 네트워크들
- Computer Vision 이외의 도메인(특히 NLP)에서도 큰 인기를 끌고 있음
    - e.g. BERT, GPT