

## 如何运行？
以下操作基于Anaconda3环境，并在macos上测试。

### 创建Python虚拟环境
```
$ conda create -n opencv python=3.6
$ activate opencv
```
### 安装OpenCV
```
$ cd modules
$ pip install opencv_python-3.4.1+contrib-cp36-cp36m-win_amd64.whl
```
### 安装dlib
```
$ pip install dlib-19.8.1-cp36-cp36m-win_amd64.whl
```
### 安装其它依赖包
```
$ cd ..
$ pip install -r requirements.txt
```
### 运行核心框架
```
$ python origin.py
```
### 运行人脸采集系统
```
$ python dataRecord.py
```
### 运行数据管理系统
```
$ python dataManage.py
```

### 退出虚拟环境
```
$ deactivate
```

### 源码修改

```
运行origin.py文件时在origin.py文件的第560行utils.viz.cv_plot_bbox的源码里，把最后一行的return img改为return class_name
运行workshop.py文件时还需要把上述的return class_name改为return img
```
