# How to set up MPII dataset
## Download annotataions
```
wget http://datasets.d2.mpi-inf.mpg.de/leonid14cvpr/mpii_human_pose_v1_u12_1.tar.gz
tar zxvf mpii_human_pose_v1_u12_1.tar.gz
```

On OSX,
```
curl -OL http://datasets.d2.mpi-inf.mpg.de/leonid14cvpr/mpii_human_pose_v1_u12_1.tar.gz
tar zxvf mpii_human_pose_v1_u12_1.tar.gz
```

## Download or link images

```
wget http://datasets.d2.mpi-inf.mpg.de/andriluka14cvpr/mpii_human_pose_v1.tar.gz
tar zxvf mpii_human_pose_v1.tar.gz
```

```
ln -s /mnt/data/MPII/images .
```



## Convert to COCO format
```
cd mpii_human_pose_v1_u12_1
python3 ../../../tool/mpii2coco.py
```

## Results
* `train.json` (16 MB)
* `test.json` (533KB)
=> Put them under `data/MPII/annotations`

