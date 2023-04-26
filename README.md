# 编译测试orb_slam2的代码

```
开发人员：杨工

工作记录：
————2023年4月27号
1、第一个版本，能编译运行
```

**系统环境**

```
ubuntu 18.04
ros melodic
```

**整体思路**

建立点云地图，跑定位，建立栅格地图，跑导航

**安装步骤**

```
安装orb_slam2深度相机版本
参考：
https://github.com/gaoxiang12/ORBSLAM2_with_pointcloud_map

cmake版本更新：
https://blog.csdn.net/weixin_42888638/article/details/125617062

编译问题：
https://blog.csdn.net/qq_15698613/article/details/98453592
https://blog.csdn.net/weixin_46808875/article/details/125317128

eigen版本问题：
https://blog.csdn.net/qq_29931565/article/details/120860674

ros编译问题：
https://blog.csdn.net/qq_42668426/article/details/108720285
```

**运行demo**

```
cd ~/orb_slam2_code/ORB_SLAM2
./Examples/RGB-D/rgbd_tum ./Vocabulary/ORBvoc.txt ./Examples/RGB-D/TUM1.yaml /home/ubuntu/bag_data/rgbd_dataset_freiburg1_xyz /home/ubuntu/bag_data/rgbd_dataset_freiburg1_xyz/associations.txt
```

**运行效果**

![Image text](https://github.com/haicheng12/orb_slam2_code/blob/main/img/test_orb_slam2.png)

