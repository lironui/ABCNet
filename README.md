#  ABCNet: Attentive Bilateral Contextual Network for Efficient Semantic Segmentation of Fine-Resolution Remote Sensing Images

⭐ [Welcome to my HomePage](https://lironui.github.io/) ⭐ 

In this repository, we implement the Attentive Bilateral Contextual Network which contains a spatial path and a contextual path to fully capture the long-range relationships and fine-grained details in fine-resolution remote sensing images. 

The detailed results can be seen in the [ABCNet: Attentive Bilateral Contextual Network for Efficient Semantic Segmentation of Fine-Resolution Remote Sensing Images](https://www.sciencedirect.com/science/article/pii/S0924271621002379).

The training and testing code can refer to [GeoSeg](https://github.com/WangLibo1995/GeoSeg).

The related repositories include:
* [MACU-Net](https://github.com/lironui/MACU-Net)->A modified version of U-Net.
* [BANet](https://github.com/lironui/BANet)->A Transformer-based segmentation network.
* [MAResU-Net](https://github.com/lironui/MAResU-Net)->A ResNet-based network with attention mechanism.
* [Multi-Attention-Network](https://github.com/lironui/Multi-Attention-Network)->A network with multi kernel attention mechanism.

If our code is helpful to you, please cite:

`R. Li, S. Zheng, C. Zhang, C. Duan, L. Wang, and P. M. Atkinson, "ABCNet: Attentive bilateral contextual network for efficient semantic segmentation of Fine-Resolution remotely sensed imagery," ISPRS Journal of Photogrammetry and Remote Sensing, vol. 181, pp. 84-98, 2021/11/01/ 2021, doi: https://doi.org/10.1016/j.isprsjprs.2021.09.005.`

Network:
------- 
![network](https://github.com/lironui/ABCNet/blob/main/figure/network.png)  
Fig. 1.  The overall architecture of ABCNet.

Result:
------- 
The result on the [UAVid dataset](https://uavid.nl/) can seen from [here, where the user name is **lironui**](https://competitions.codalab.org/competitions/25224#results) or [here](https://competitions.codalab.org/competitions/public_submissions/25224) and can be downloaded by [**this link**](https://competitions.codalab.org/my/competition/submission/904615/input.zip):

| Method    | building | tree     | clutter   | road     | vegetation | static car | moving car | human    | mIoU     | 
|-----------|----------|----------|-----------|----------|------------|------------|------------|----------|----------| 
| MSD       | 79.8     | 74.5     | 57.0      | 74.0     | 55.9       | 32.1       | 62.9       | **19.7** | 57.0     | 
| Fast-SCNN | 75.7     | 71.5     | 44.2      | 61.6     | 43.4       | 19.5       | 51.6       | 0.0      | 45.9     | 
| BiSeNet   | 85.7     | 78.3     | 64.7      | 61.1     | **77.3**   | **63.4**   | 48.6       | 17.5     | 61.5     | 
| SwiftNet  | 85.3     | 78.2     | 64.1      | 61.5     | 76.4       | 62.1       | 51.1       | 15.7     | 61.1     | 
| ShelfNet  | 76.9     | 73.2     | 44.1      | 61.4     | 43.4       | 21.0       | 52.6       | 3.6      | 47.0     |  
| ABCNet    | **86.4** | **79.9** | **67.4**  | **81.2** | 63.1       | 48.4       | **69.8**   | 13.9     | **63.8** | 


![Result](https://github.com/lironui/ABCNet/blob/main/figure/UAVid.png)  
Fig. 2.  The experimental results on the UAVid test set. The first column illustrates the input RGB images, the second column depicts the outputs of MSD and the third column shows the predictions of our ABCNet. 

