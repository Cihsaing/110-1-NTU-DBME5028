# 110-1-NTU-DBME5028
Midterm Project : Hard task - Intracranial Hemorrhage prediction \
Teem members:\
r09942171 黃繼綸 \
f09921058 陳羿翔

# Environment
OS : Ubuntu 16.04 \
Python36

# Requirements
1. torch 1.3.1+
2. grad-cam 
3. opencv 4.5
4. tensorboradX
5. tqdm

# How to use
### Download the models
```bash
$ bash download.sh
```

### Training from scratch
SEresnet50 training
```bash
$ python train.py --data_path ../dataset --n_cpu 8 --batch_size 48 --model SEresnet50 --saved_name model_SEresnet50
```

resnext50 training
```bash
$ python train.py --data_path ../dataset --n_cpu 8 --batch_size 64 --model resnext50 --saved_name model_resnext50
```

### Testing
```bash
$ python inference.py --data_path ../dataset --output ./output.csv
```


