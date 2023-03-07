# UNet-Segmantation
Public Dataset：DRIVE（Digital Retinal Images for Vessel Extraction）


## Dataset
DRIVE（Digital Retinal Images for Vessel Extraction）数据集是用于血管分割（vessel segmentation）任务的一个公共数据集。该数据集包含40张人类眼底图像，其中20张用于训练，另外20张用于测试。

DRIVE数据集中的每张图像的分辨率为 565 x 584 像素，并且每张图像都包含一个视网膜区域，其中包含了视网膜血管和周围组织的信息。每张图像都带有与之对应的手动标注图（ground truth），其中包含了视网膜血管的二值化信息，可以用于模型的训练和评估。

DRIVE数据集在计算机视觉领域中被广泛用于血管分割算法的评估和比较。由于其包含了高质量的手动标注信息，因此它通常被认为是一个很好的数据集，可用于评估血管分割算法的性能。

## Model
本项目采用经典UNet网络模型。
U-Net是一种常用于图像分割的卷积神经网络（Convolutional Neural Network，CNN）。它最初由欧洲卫生研究所（European Molecular Biology Laboratory，EMBL）的Ronneberger等人在2015年提出，主要用于分割医学图像中的器官和病变。

U-Net网络的主要特点是具有“U”字型的结构。它包含两个部分：下采样路径（encoding path）和上采样路径（decoding path）。其中，下采样路径使用卷积和池化层逐渐减少图像的尺寸和通道数，从而提取出图像的局部特征；上采样路径使用反卷积和上采样操作逐步恢复图像的尺寸和通道数，并将局部特征与全局信息相结合，得到最终的分割结果。

在U-Net中，还引入了跳跃连接（skip connection）的概念。跳跃连接是将下采样路径中的某些层和上采样路径中对应的层相连，从而使得上采样路径可以利用下采样路径中更多的低级特征信息，提高分割的准确性和鲁棒性。

U-Net网络的优点在于，它可以通过少量的训练数据就能够获得较好的分割效果，而且在分割任务中具有较高的准确性和鲁棒性。因此，它被广泛应用于医学图像处理、自然图像分割等领域。
![image](https://user-images.githubusercontent.com/92668045/223342415-c360d326-bb3f-47ed-904a-49d0b13df461.png)
