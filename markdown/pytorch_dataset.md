### What we need now

- 1.Read & Split(Dataset)
    - 1)Read tabular dataset (e.g. csv file)
    - 2)Shuffling before split into train/valid/test set
    - 3)Split train, valid and test set
- 2.Preprocessing(Dataset)
    - 1)Remove unnecessary rows (e.g. high null ratio)
    - 2)Standard or Min/Max Scaling based on training set
- 3.Iterator(DataLoader)
    - 1)Shuffle for each epoch
    - 2)Get tensor chunk with mini-batch size
    - 3)Yield the mini-batch for each iteration

### Plug & Play

- torch.utils.data.Dataset
    - __init__(self, *args, **kwargs): 데이터를 읽어오기
    - __len__(self): 데이터의 크기 알기
    - __getitem__(self, idx): 전처리 및 미니배치를 위한 샘플을 변환 
- torch.utils.data.DataLoader
    - 셔플링, 미니배치 구성, Yield