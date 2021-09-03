#  Bilateral Awareness Network

In this repository, we implement the Bilateral Awareness Network which contains a dependency path and a texture path to fully capture the long-range relationships and fine-grained details in very fine resolution (VFR) urban scene images . 

The detailed results can be seen in the [Multi-stage Attention ResU-Net for Semantic Segmentation of Fine-Resolution Remote Sensing Images](https://arxiv.org/ftp/arxiv/papers/2106/2106.12413.pdf).

The related repositories include:
* [MACU-Net](https://github.com/lironui/MACU-Net)->A modified version of U-Net.
* [MAResU-Net](https://github.com/lironui/MAResU-Net)->A ResNet-based network with attention mechanism.
* [Multi-Attention-Network](https://github.com/lironui/Multi-Attention-Network)->A network with multi kernel attention mechanism.

If our code is helpful to you, please cite:

`Wang, L., Li, R., Wang, D., Duan, C., Wang, T., & Meng, X. (2021). Transformer Meets Convolution: A Bilateral Awareness Net-work for Semantic Segmentation of Very Fine Resolution Ur-ban Scene Images. arXiv preprint arXiv:2106.12413.`

Requirements：
------- 
```
numpy >= 1.16.5
PyTorch >= 1.3.1
sklearn >= 0.20.4
tqdm >= 4.46.1
imageio >= 2.8.0
```

Network:
------- 
![network](https://github.com/lironui/MAResU-Net/blob/main/Fig/network.png)  
Fig. 1.  The structure of (a) the proposed MAResU-Net and (b) the attention block.

Result:
------- 
The result on the [UAVid dataset](https://uavid.nl/) can seen from [here, where the user name is **AlexWang**](https://competitions.codalab.org/competitions/25224#results).
![Result](https://github.com/lironui/MAResU-Net/blob/main/Fig/result.png)  
Fig. 2. Visualization of results on the Vaihingen.

Complexity:
------- 
![Complexity](https://github.com/lironui/MAResU-Net/blob/main/Fig/complexity.png)  
Fig. 3. The (a) computation requirement and (b) memory requirement of the raw dot-product attention mechanism and the proposed linear attention mechanism under different input sizes. Please notice that the figure is in log scale.
