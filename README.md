# UNet-Segmantation
Public Dataset：DRIVE（Digital Retinal Images for Vessel Extraction）


## Dataset
DRIVE（Digital Retinal Images for Vessel Extraction）数据集是用于血管分割（vessel segmentation）任务的一个公共数据集。该数据集包含40张人类眼底图像，其中20张用于训练，另外20张用于测试。

DRIVE数据集中的每张图像的分辨率为 565 x 584 像素，并且每张图像都包含一个视网膜区域，其中包含了视网膜血管和周围组织的信息。每张图像都带有与之对应的手动标注图（ground truth），其中包含了视网膜血管的二值化信息，可以用于模型的训练和评估。

DRIVE数据集在计算机视觉领域中被广泛用于血管分割算法的评估和比较。由于其包含了高质量的手动标注信息，因此它通常被认为是一个很好的数据集，可用于评估血管分割算法的性能。

## Model
使用经典UNet网络
![image](https://user-images.githubusercontent.com/92668045/223342415-c360d326-bb3f-47ed-904a-49d0b13df461.png)
