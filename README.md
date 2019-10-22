# 无人驾驶车车道线检测项目（Lane-Finding-Project）
无人驾驶车车道线检测项目（Lane Finding Project）
## 车道线检测项目

本项目来自优达学城无人驾驶车课程，项目目标基于计算机视觉方法实现车道线检测与显示的效果。
项目链接：https://github.com/udacity/CarND-Advanced-Lane-Lines

项目实现
---
具体实现方式：
* 计算摄像机的校准矩阵与畸变系数（借助已有的黑白棋盘图像）
* 对原始图像应用失真校正
* 应用颜色转换，梯度等手段对图像处理得到一个阈值化的二进制图像
* 应用透视变化技术将二进制图像转换视角得到鸟瞰视角图（"birds-eye view"）
* 检测二进制图像的车道像素并进行拟合以找到车道边界
* 确定计算得到车道的曲率
* 将检测到的车道边界与回原始图像叠加
* 可视化显示车道边界以及车道曲率
