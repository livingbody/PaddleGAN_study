# PaddleGAN七日打卡营

《百度飞桨生成对抗网络七日打卡营》，PaddlePaddle研发团队直播授课，4月15日起，每天1小时，连续7天，深入剖析多种经典及前沿 GAN 模型算法及代码。

直播链接：http://live.bilibili.com/21689802


致敬开源、鼓励分享：开课期间发布原创优秀技术经验贴、有价值的项目、视频等，即可获得额外加分，加分直接体现在总成绩上。希望你收获更强的自己，如有问题，欢迎加入课程qq群（651940985）交流讨论。

## 课程安排

4月15日 20：30~21：30：Day 1 GAN基础概念及应用介绍

4月16日 20：30~21：30：Day 2 GAN的技术演进及人脸生成应用

4月17日 20：30~21：30：Day 3 图像翻译及卡通画应用

4月18日 20：30~21：30：Day 4 超分辨率及老视频修复

4月19日 20：30~21：30：Day 5 动作迁移理论及实践

4月20日 20：30~21：30：Day 6 Wav2lip唇形合成理论及趣味应用

4月22日 19：00~20：00：Day 7 作业讲评与拓展提升

## 作业

作业提交规则：作业提交均在AI Studio上，前5天的作业的截止提交日期均在第二天课程开始前，第6天的大作业将预留一天时间给大家完成，在结营前完成即可。

作业评讲：每日作业评讲均在第二天的课程开头10min。

**Bonus🤩：鼓励大家除了在AI Studio上完成作业外，也可自行创建GitHub repo，在repo上完成作业（内容可和AI Studio一样），并将PaddleGAN加入你的repo的requirements.txt中，最后将repo链接放在AI Studio项目中即可获得加分，最终有机会获得大奖°˖✧◝(⁰▿⁰)◜✧˖°。**

Day 1：[客观题_理论层面的单选题](./homework1/homework1.md) 

Day 2：[代码题_基于DCGAN，改写为LS-GAN](./homework2/homework2.md) 

Day 3：[代码题_填空补全基于pix2pix实现人脸卡通的预测代码](./homework3/第三节课pix2pix人像卡通化.md) 

Day 4：[客观题+项目展示（照片、视频）](./homework4/第四课代码题老视频修复.md)

Day 5：[客观题+项目展示（照片、视频）](./homework5/第五课图像超分客观题.md)

Day 6：[大作业：自选PaddleGAN里面的模型实现超分](./homework6/homework6.md)

## 奖品列表

### 反正很好看，虽然没有，但是想看看！！！
### 有奖品不要，哎，咱就是玩，哈哈哈！！！

一等奖1名：HHKB Professional静电容蓝牙键盘

![04a0a06a4b03b679100c02a4463ccf47](https://user-images.githubusercontent.com/48054808/113859231-40736800-97d7-11eb-90e9-f4d371a8067c.png)

二等奖2名：Kindle paperwhite 电子阅读器

![db5121b665d75b9929d5221a653ec84c](https://user-images.githubusercontent.com/48054808/113859313-54b76500-97d7-11eb-9012-49712d03a41e.png)

三等奖6名：小度无线智能耳机

![9e31104e40d1b74ad99d5983d77f4b86](https://user-images.githubusercontent.com/48054808/113859359-64cf4480-97d7-11eb-8881-83d493c970a4.png)

优秀奖10名：纸质书_《Generative Deep Learning》+《Deep Learning》

完成课程的同学还将获得我们精美的结业证书！

![ea5b03930f1c8fd4d9991c8c78694cb2](https://user-images.githubusercontent.com/48054808/113859475-86c8c700-97d7-11eb-8bd5-ee90bdeaad6f.png)

## 相关模型资料

以下是课程中所涉及到的所有模型简介、代码链接及论文。

***注意：实际代码请参考Config文件进行配置。**

### Wasserstein GAN

论文：[Wasserstein GAN](https://arxiv.org/pdf/1701.07875.pdf)
简介：本文从理论上分析了原始 GAN 模型存在的训练不稳定、生成器和判别器的 loss 无法只是训练进程、生成样本缺乏多样性等问题，并通过改进算法流程针对性的给出了改进要点。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/wgan_mnist.yaml

### DCGAN

论文：[UNSUPERVISED REPRESENTATION LEARNING WITH DEEP CONVOLUTIONAL GENERATIVE ADVERSARIAL NETWORKS](https://arxiv.org/pdf/1511.06434.pdf)
简介：由于卷积神经网络(Convolutional neural network, CNN)比MLP有更强的拟合与表达能力，并在判别式模型中取得了很大的成果。因此，本文将CNN引入生成器和判别器，称作深度卷积对抗神经网络（Deep Convolutional GAN, DCGAN）。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/dcgan_mnist.yaml

### Least Squares GAN

论文：[Least Squares Generative Adversarial Networks](https://arxiv.org/pdf/1611.04076.pdf)
简介：本文主要将交叉熵损失函数换做了最小二乘损失函数，改善了传统 GAN 生成的图片质量不高，且训练过程十分不稳定的问题。

### Progressive Growing of GAN

论文：[PROGRESSIVE GROWING OF GANS FOR IMPROVED QUALITY, STABILITY, AND VARIATION](https://arxiv.org/pdf/1710.10196.pdf)
简介：本文提出了一种用来训练生成对抗网络的新方法：渐进式地增加生成器和判别器的规模，同时，提出了一种提高生成图像多样性的方法以及给出一种新的关于图像生成质量和多样性的评价指标。

### StyleGAN

论文：[A Style-Based Generator Architecture for Generative Adversarial Networks](https://arxiv.org/pdf/1812.04948.pdf)
简介：本文是NVIDIA继ProGAN之后提出的新的生成网络，其主要通过分别修改每一层级的输入，在不影响其他层级的情况下，来控制该层级所表示的视觉特征。 这些特征可以是粗的特征（如姿势、脸型等），也可以是一些细节特征（如瞳色、发色等）。

### StyleGAN2

论文：[Analyzing and Improving the Image Quality of StyleGAN](https://arxiv.org/pdf/1912.04958.pdf)
简介：本文主要解决StyleGAN生成图像伪影的同时还能得到细节更好的高质量图像。新的改进方案也不会带来更高的计算成本。不管是在现有的分布质量指标上，还是在人所感知的图像质量上，新提出的模型都实现了无条件图像建模任务上新的 SOTA。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/stylegan_v2_256_ffhq.yaml

### Conditional GAN

论文：[Conditional Generative Adversarial Nets](https://arxiv.org/pdf/1411.1784.pdf)
简介：本文提出在利用 GAN（对抗网络）的方法时，在生成模型G和判别模型D中都加入条件信息来引导模型的训练，并将这种方法应用于跨模态问题，例如图像自动标注等。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/cond_dcgan_mnist.yaml

### CycleGAN

论文：[Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/pdf/1703.10593.pdf)
 简介：CycleGAN本质上是两个镜像对称的GAN，构成了一个环形网络。 两个GAN共享两个生成器，并各自带一个判别器，即共有两个判别器和两个生成器。 一个单向GAN两个loss，两个即共四个loss。 可以实现无配对的两个图片集的训练是CycleGAN与Pixel2Pixel相比的一个典型优点。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/cyclegan_horse2zebra.yaml

### Pix2Pix

论文：[Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/pdf/1611.07004.pdf)
简介：本文在GAN的基础上提供一个通用方法，完成成对的图像转换。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/pix2pix_cityscapes_2gpus.yaml

### U-GAT-IT

论文：[U-GAT-IT: UNSUPERVISED GENERATIVE ATTENTIONAL NETWORKS WITH ADAPTIVE LAYERINSTANCE NORMALIZATION FOR IMAGE-TO-IMAGE TRANSLATION](https://arxiv.org/pdf/1907.10830.pdf)
简介：本文主要研究无监督的image-to-image translation。在风格转换中引入了注意力模块，并且提出了一种新的可学习的normalization方法。注意力模块根据辅助分类器获得的attention map，使得模型聚能更好地区分源域和目标域的重要区域。同时，AdaLIN（自适应层实例归一化）帮助注意力指导模型根据所学习的数据集灵活地控制形状和纹理的变化量。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/ugatit_selfie2anime_light.yaml

### Super Resolution GAN

论文：[Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network](https://arxiv.org/pdf/1609.04802.pdf)
简介：本文主要讲解如何利用卷积神经网络实现单影像的超分辨率，其瓶颈仍在于如何恢复图像的细微纹理信息。

### Enhanced Super Resolution GAN

论文：[ESRGAN: Enhanced Super-Resolution Generative Adversarial Networks](https://arxiv.org/pdf/1809.00219.pdf)
简介：本文在SRGAN的基础上进行了改进，包括改进网络的结构，判决器的判决形式，以及更换了一个用于计算感知域损失的预训练网络。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/esrgan_x4_div2k.yaml

### Residual Channel Attention Networks（RCAN）

论文：[Image Super-Resolution Using Very Deep Residual Channel Attention Networks](https://arxiv.org/pdf/1807.02758.pdf)
简介：本文提出了一个深度残差通道注意力网络（RCAN）解决过深的网络难以训练、网络的表示能力较弱的问题。

### EDVR

论文：[EDVR: Video Restoration with Enhanced Deformable Convolutional Networks](https://arxiv.org/pdf/1905.02716.pdf)
简介：本文主要介绍基于可形变卷积的视频恢复、去模糊、超分的网络。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/edvr.yaml

### First Order Motion

论文：[First Order Motion Model for Image Animation](https://arxiv.org/pdf/2003.00196.pdf)
简介：本文介绍的是image animation，给定一张源图片，给定一个驱动视频，生成一段视频，其中主角是源图片，动作是驱动视频中的动作。如下图所示，源图像通常包含一个主体，驱动视频包含一系列动作。

### Wav2lip

论文：[A Lip Sync Expert Is All You Need for Speech to Lip Generation In The Wild](https://arxiv.org/pdf/2008.10010.pdf)
简介：本文主要介绍如何将任意说话的面部视频与任意语音进行唇形同步。

代码链接：https://github.com/PaddlePaddle/PaddleGAN/blob/develop/configs/wav2lip.yaml


## 优秀作业公示

没有我

## 奖品名单公布

没有我


