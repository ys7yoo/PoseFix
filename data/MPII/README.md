# Get annotations
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

## Convert to COCO format
```
cd mpii_human_pose_v1_u12_1
python3 ../../../tool/mpii2coco.py
```

## Results

