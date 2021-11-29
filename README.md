# 110-1-NTU-DBME5028
Midterm Project : Hard task - Intracranial Hemorrhage prediction \
Teem members:\
r09942171 黃繼綸 \
rxxxxxxxx 陳羿翔

# How to use this code
### Download the models
```bash
$ bash download.sh
```

### Training
```bash
$ python train.py --data_path ../dataset
```

### Testing
```bash
$ python inference.py --data_path ../dataset ./output.csv
```

