# Image-Processing-exm

Coure project for Image Processing

## 项目要求

详情可以看作业要求文档

## 解决思路

1. 在原始图像上分割得到肺实质区域

对于一般情况，由于肺部的肺实质区域是白色的，实质区域是黑色的，观察图像可以得出应该只需要将图像的黑白区域进行分离即可，即只需要保留图像中灰度值较黑的区域。

然而不难发现我们还需要对特殊情况进行处理，由于病灶区域的灰度值与肺实质区域非常相近（都为白色），如果我们不对上述算法进行改进，那么我们将会误把原本属于肺部实质区域的病灶区域一并去除掉，这并不符合我们的目标，因此需要想出新的方法来将灰度值相近的病灶区域与肺部的非实质区域区分开来。
