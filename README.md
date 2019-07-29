# SEU-Advanced-Vision

## 算法

### LINEMOD 数据集制作

数据集制作工具[*ObjectDatasetTools*](https://github.com/seu-labview/ObjectDatasetTools)

### 神经网络

前期选用[*YOLO6D*](https://github.com/seu-labview/singleshot6Dpose)

## 前端

使用*PyQt*完成前端设计

## 接口

使用*librealsense2*调用SR300

### SR300 查看相机内参

使用*rs-sensor-control*  [*细节*](https://blog.csdn.net/weixin_39585934/article/details/84147449)

## 项目结构

`QT.py`为主文件，实现了整个项目的运作，包含前端显示、调用神经网络、保存文件等。

`Predict.py`为神经网络接口，被`QT.py`调用。

`MeshPly.py`为3D模型接口，被`Predict.py`调用。

使用时，将`LINEMOD`文件夹置于本项目根目录。