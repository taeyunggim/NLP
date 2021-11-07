### Summary

- MLE를 통해 수집한 데이터셋을 잘 설명하는 확률 분포의 파라미터를 찾을 수 있음
- Neural Networks 또한 확률 분포 함수이므로 MLE를 통해 파라미터를 찾을 것
    - 최대화 대신 최소화를 위해 Negative-Log-Likelihood (NLL)을 Gradient Descent
- Gradient Descent를 수행하기 위해선, 파라미터에 대한 미분이 필요함
    - 이를 효율적으로 수행하기 위해 back-propagation을 활용