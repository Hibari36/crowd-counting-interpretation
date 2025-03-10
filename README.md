# Awesome Crowd Counting[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

If you have any problems, suggestions or improvements, please submit the issue or PR.

## Contents
* [Misc](#misc)
* [Datasets](#datasets)
* [Papers](#papers)
* [Leaderboard](#leaderboard)
* [Classification](#classification)

## Misc

### News
- [2022.09] The VSCrowd Dataset is released.
- [2022.01] The FUDAN-UCC Dataset is released.
- [2021.04] The RGBT-CC Benchmark is released.
- [2020.04] The JHU-CROWD++ Dataset is released.
- [2020.01] The NWPU-Crowd benchmark is released.

### Call for Papers
- [Transportation Research Part C] Special Issue on: Applications of artificial intelligence, computer vision, physics and econometrics modelling methods in pedestrian traffic modelling and crowd safety [[Link](https://www.sciencedirect.com/journal/transportation-research-part-c-emerging-technologies/about/call-for-papers#call-for-papers-applications-of-artificial-intelligence-computer-vision-physics-and-econometrics-modelling-methods-in-pedestrian-traffic-modelling-and-crowd-safety)]. Deadline: April 30th, 2023.
- [IET Image Processing] ~~Special Issue on: Crowd Understanding and Analysis~~ [[Link](https://digital-library.theiet.org/content/journals/iet-ipr/info/spl-issues;jsessionid=rfnb4mhi25p6.x-iet-live-01)] [[PDF](https://digital-library.theiet.org/files/IET_IPR_CFP_CUA.pdf)]

### Challenge
- [[NWPU-Crowd Counting](https://www.crowdbenchmark.com/nwpucrowd.html)] Crowd counting. Deadline: none.
- [[VisDrone 2021](http://aiskyeye.com/challenge_2021/crowd-counting-2/)] ~~Crowd counting. ICCV Workshop. Deadline: **2021.07.15**.~~
- [[VisDrone 2020](http://aiskyeye.com/challenge/crowd-counting/)] ~~Crowd counting. ECCV Workshop. Deadline: **2020.07.15**.~~

### Code
- [[C^3 Framework](https://github.com/gjy3035/C-3-Framework)] An open-source PyTorch code for crowd counting, which is released. ![GitHub stars](https://img.shields.io/github/stars/gjy3035/C-3-Framework.svg?logo=github&label=Stars)
- [[CCLabeler](https://github.com/Elin24/cclabeler)] A web tool for labeling pedestrians in an image, which is released. ![GitHub stars](https://img.shields.io/github/stars/Elin24/cclabeler.svg?logo=github&label=Stars)

### Technical blog
- [Chinese Blog] 人群计数论文解读 [[Link](https://zhuanlan.zhihu.com/c_1111215695622352896)]
- [2019.05] [Chinese Blog] C^3 Framework系列之一：一个基于PyTorch的开源人群计数框架 [[Link](https://zhuanlan.zhihu.com/p/65650998)]
- [2019.04] Crowd counting from scratch [[Link](https://github.com/CommissarMa/Crowd_counting_from_scratch)]
- [2017.11] Counting Crowds and Lines with AI [[Link1](https://blog.dimroc.com/2017/11/19/counting-crowds-and-lines/)] [[Link2](https://count.dimroc.com/)] [[Code](https://github.com/dimroc/count)]![GitHub stars](https://img.shields.io/github/stars/dimroc/count.svg?logo=github&label=Stars)

###  GT generation
- Density Map Generation from Key Points [[Matlab Code](https://github.com/aachenhang/crowdcount-mcnn/tree/master/data_preparation)] [[Python Code](https://github.com/leeyeehoo/CSRNet-pytorch/blob/master/make_dataset.ipynb)] [[Fast Python Code](https://github.com/vlad3996/computing-density-maps)] [[Pytorch CUDA Code](https://github.com/gjy3035/NWPU-Crowd-Sample-Code/blob/master/misc/dot_ops.py)]

### Related Tasks
Crowd Analysis, [Crowd Localization](https://github.com/taohan10200/Awesome-Crowd-Localization), [Video Surveillance](https://github.com/CommissarMa/Awesome-Public-Safety-in-Vision), Dense/Small/Tiny Object Detection

## Datasets

Please refer to [this page](src/Datasets.md).

## Papers

Considering the increasing number of papers in this field, we roughly summarize some articles and put them into the following categories (they are still listed in this document):

| [[**Top Conference/Journal**](src/Top_Conference-Journal.md)] | [[**Survey**](src/Survey.md)] | [[**Un-/semi-/weakly-/self- Supervised Learning**](src/Un-_Semi-_Weakly-_Self-_supervised_Learning.md)] |
| :---- | :---- | :---- |
| [[**Auxiliary Tasks**](src/Auxiliary_Tasks.md)] | [[**Localization**](src/Localization.md)] | [[**Transfer Learning and Domain Adaptation**](src/Transfer_Learning_and_Domain_Adaptation.md)] |
| [[**Light-weight Models**](src/Light-weight_Model.md)] | [[**Video**](src/Video.md)] | [[**Network Design, Search**](src/Network_Design_and_Search.md)] |
| [[**Perspective Map**](src/Perspective_Map.md)] | [[**Attention**](src/Attention.md)] | [[**Transformer**](src/Transformer.md)] |

### arXiv papers
Note that all unpublished arXiv papers are not included in [the leaderboard of performance](#performance).

- LCDnet: A Lightweight Crowd Density Estimation Model for Real-time Video Surveillance [[paper](https://arxiv.org/abs/2302.05374)]

    #### ～～Video Crowd Counting skipped～～
    #### supplement: it seems not to contain many highlights.
    ***
- GCNet: Probing Self-Similarity Learning for Generalized Counting Network [[paper](https://arxiv.org/abs/2302.05132)]

    #### A paper for similar object counting with one-shot example.
    ***

- A Unified Object Counting Network with Object Occupation Prior [[paper](https://arxiv.org/abs/2212.14193)]

    #### the task encounter newly coming data in real world called evolving crowd counting.
    ***
- Mask Focal Loss for dense crowd counting with canonical object detection networks [[paper](https://arxiv.org/abs/2212.11542)]

    #### defined a mask focal loss to perform dense crowd counting with canonical object detection network.
    ***
- CountingMOT: Joint Counting, Detection and Re-Identification for Multiple Object Tracking [[paper](https://arxiv.org/abs/2212.05861)]

    #### proposed a new task, counting, detection and re-id, called CountingMOT, applied in crowded scene.
    ***
- Progressive Multi-resolution Loss for Crowd Counting [[paper](https://arxiv.org/abs/2212.04127)]

    #### proposed a new L2 Loss meassuring predicted single density map at different scales and proved mathematically traditional L2 loss is its sub-optimal form.
    ***
- Counting Like Human: Anthropoid Crowd Counting on Modeling the Similarity of Objects [[paper](https://arxiv.org/abs/2212.02248)]

    #### it requires anthropoid crowd counting with detect the key similarity between objects.
    ***
- DASECount: Domain-Agnostic Sample-Efficient Wireless Indoor Crowd Counting via Few-shot Learning [[paper](https://arxiv.org/abs/2211.10040)]

    #### emmmm, what to say, just like its title, it is clear~
    *** 
- DroneNet: Crowd Density Estimation using Self-ONNs for Drones [[paper](https://arxiv.org/abs/2211.07137)]

    #### it seem not to contain any highlights.
    #### However, it reminds me of two drone datasets.
    #### Real Trash!!!! It is a waste of time!!!!
    ***
- Scale-Aware Crowd Counting Using a Joint Likelihood Density Map and Synthetic Fusion Pyramid Network [[paper](https://arxiv.org/abs/2211.06835)]

    #### proposed a loss function to model the annotation error as a guassian distribution and......
    ***
- Inception-Based Crowd Counting -- Being Fast while Remaining Accurate [[paper](https://arxiv.org/abs/2210.09796)]

    #### proposed inception-V3 to decrease the calculation and maintain the accuracy
    ***
- Crowd Counting on Heavily Compressed Images with Curriculum Pre-Training [[paper](https://arxiv.org/abs/2208.07075)]

    #### emmmm, special field and implicit target. No more explaination.
    ***
- MAFNet: A Multi-Attention Fusion Network for RGB-T Crowd Counting [[paper](https://arxiv.org/abs/2208.06761)]

    #### A fution network for RGB and thermal image data.
    #### its fusion method: seems normal and no more research~
    ***
- Multi-scale Feature Aggregation for Crowd Counting [[paper](https://arxiv.org/abs/2208.05256)]

    #### multi-feature aggregation with short connection and skip connnection
    #### seems its structure is too simple and it is compared with CVPR2020emmmm
    ***
- Redesigning Multi-Scale Neural Network for Crowd Counting [[paper](https://arxiv.org/abs/2208.02894)][[code](https://github.com/ZPDu/Redesigning-Multi-Scale-Neural-Network-for-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/ZPDu/Redesigning-Multi-Scale-Neural-Network-for-Crowd-Counting.svg?logo=github&label=Stars)

    #### designs many complicated structures to solve the scaling problem
    #### merge multi-scale feature, expert scheme, soft gating and loss fuc. 
    ***

<details>
<summary>Earlier ArXiv Papers</summary>
- Analysis of the Effect of Low-Overhead Lossy Image Compression on the Performance of Visual Crowd Counting for Smart City Applications [[paper](https://arxiv.org/abs/2207.10155)]
- Counting Varying Density Crowds Through Density Guided Adaptive Selection CNN and Transformer Estimation [[paper](https://arxiv.org/abs/2206.10075)]
- Indirect-Instant Attention Optimization for Crowd Counting in Dense Scenes [[paper](https://arxiv.org/abs/2206.05648)]
- Reducing Capacity Gap in Knowledge Distillation with Review Mechanism for Crowd Counting [[paper](https://arxiv.org/abs/2206.05475)]
- Glance to Count: Learning to Rank with Anchors for Weakly-supervised Crowd Counting [[paper](https://arxiv.org/abs/2205.14659)]
- Forget Less, Count Better: A Domain-Incremental Self-Distillation Learning Benchmark for Lifelong Crowd Counting [[paper](https://arxiv.org/abs/2205.03307)]
- Counting in the 2020s: Binned Representations and Inclusive Performance Measures for Deep Crowd Counting Approaches [[paper](https://arxiv.org/abs/2204.04653)]
- CrowdMLP: Weakly-Supervised Crowd Counting via Multi-Granularity MLP [[paper](https://arxiv.org/abs/2203.08219)]
- Joint CNN and Transformer Network via weakly supervised Learning for efficient crowd counting [[paper](https://arxiv.org/abs/2203.06388)]
- Counting with Adaptive Auxiliary Learning [[paper](https://arxiv.org/abs/2203.04061)][[code](https://github.com/smallmax00/Counting_With_Adaptive_Auxiliary_Learning)]![GitHub stars](https://img.shields.io/github/stars/smallmax00/Counting_With_Adaptive_Auxiliary_Learning.svg?logo=github&label=Stars)
- CrowdFormer: Weakly-supervised Crowd counting with Improved Generalizability [[paper](https://arxiv.org/abs/2203.03768)]
- A Unified Multi-Task Learning Framework of Real-Time Drone Supervision for Crowd Counting [[paper](https://arxiv.org/abs/2202.03843)]
- S2FPR: Crowd Counting via Self-Supervised Coarse to Fine Feature Pyramid Ranking [[paper](https://arxiv.org/abs/2201.04819)][[code](https://github.com/bridgeqiqi/S2FPR)]![GitHub stars](https://img.shields.io/github/stars/bridgeqiqi/S2FPR.svg?logo=github&label=Stars)
- Scene-Adaptive Attention Network for Crowd Counting [[paper](https://arxiv.org/abs/2112.15509)]
- Object Counting: You Only Need to Look at One [[paper](https://arxiv.org/abs/2112.05993)]
- PANet: Perspective-Aware Network with Dynamic Receptive Fields and Self-Distilling Supervision for Crowd Counting [[paper](https://arxiv.org/abs/2111.00406)]
- LDC-Net: A Unified Framework for Localization, Detection and Counting in Dense Crowds [[paper](https://arxiv.org/abs/2110.04727)]
- CCTrans: Simplifying and Improving Crowd Counting with Transformer [[paper](https://arxiv.org/abs/2109.14483)]
- S4-Crowd: Semi-Supervised Learning with Self-Supervised Regularisation for Crowd Counting [[paper](https://arxiv.org/abs/2108.13969)]
- Fine-grained Domain Adaptive Crowd Counting via Point-derived Segmentation [[paper](https://arxiv.org/abs/2108.02980)]
- Reducing Spatial Labeling Redundancy for Semi-supervised Crowd Counting [[paper](https://arxiv.org/abs/2108.02970)]
- Video Crowd Localization with Multi-focus Gaussian Neighbor Attention and a Large-Scale Benchmark [[paper](https://arxiv.org/abs/2107.08645)]
- Multi-Level Attentive Convoluntional Neural Network for Crowd Counting [[paper](https://arxiv.org/abs/2105.11422)]
- Boosting Crowd Counting with Transformers [[paper](https://arxiv.org/abs/2105.10926)]
- Crowd Counting by Self-supervised Transfer Colorization Learning and Global Prior Classification [[paper](https://arxiv.org/abs/2105.09684)]
- WheatNet: A Lightweight Convolutional Neural Network for High-throughput Image-based Wheat Head Detection and Counting [[paper](https://arxiv.org/abs/2103.09408)]
- Motion-guided Non-local Spatial-Temporal Network for Video Crowd Counting [[paper](https://arxiv.org/abs/2104.13946)]
- Multi-channel Deep Supervision for Crowd Counting [[paper](https://arxiv.org/abs/2103.09553)]
- Enhanced Information Fusion Network for Crowd Counting [[paper](https://arxiv.org/abs/2101.01479)]
- Scale-Aware Network with Regional and Semantic Attentions for Crowd Counting under Cluttered Background [[paper](https://arxiv.org/abs/2101.04279)]
- Learning Independent Instance Maps for Crowd Localization [[paper](https://arxiv.org/abs/2012.04164)] [[code](https://github.com/taohan10200/IIM)]![GitHub stars](https://img.shields.io/github/stars/taohan10200/IIM.svg?logo=github&label=Stars)
- PSCNet: Pyramidal Scale and Global Context Guided Network for Crowd Counting [[paper](https://arxiv.org/abs/2012.03597)]
- A Strong Baseline for Crowd Counting and Unsupervised People Localization [[paper](https://arxiv.org/abs/2011.03725)]
- A Study of Human Gaze Behavior During Visual Crowd Counting [[paper](https://arxiv.org/abs/2009.06502)]
- Bayesian Multi Scale Neural Network for Crowd Counting [[paper](https://arxiv.org/abs/2007.14245)]
- Dense Crowds Detection and Counting with a Lightweight Architecture [[paper](https://arxiv.org/abs/2007.06630)]
- Exploit the potential of Multi-column architecture for Crowd Counting [[paper](https://arxiv.org/abs/2007.05779)][[code](https://github.com/JunhaoCheng/Pyramid_Scale_Network)]![GitHub stars](https://img.shields.io/github/stars/JunhaoCheng/Pyramid_Scale_Network.svg?logo=github&label=Stars)
- Recurrent Distillation based Crowd Counting [[paper](https://arxiv.org/abs/2006.07755)]
- Ambient Sound Helps: Audiovisual Crowd Counting in Extreme Conditions [[paper](https://arxiv.org/abs/2005.07097)][[code](https://github.com/qingzwang/AudioVisualCrowdCounting)]![GitHub stars](https://img.shields.io/github/stars/qingzwang/AudioVisualCrowdCounting.svg?logo=github&label=Stars)
- CNN-based Density Estimation and Crowd Counting: A Survey [[paper](https://arxiv.org/abs/2003.12783)]
- Drone Based RGBT Vehicle Detection and Counting: A Challenge [[paper](https://arxiv.org/abs/2003.02437)]
- From Open Set to Closed Set: Supervised Spatial Divide-and-Conquer for Object Counting [[paper](https://arxiv.org/abs/2001.01886)](extension of [S-DCNet](#S-DCNet))
- Drone-based Joint Density Map Estimation, Localization and Tracking with Space-Time Multi-Scale Attention Network [[paper](https://arxiv.org/abs/1912.01811)][[code](https://github.com/VisDrone)]
- Using Depth for Pixel-Wise Detection of Adversarial Attacks in Crowd Counting [[paper](https://arxiv.org/abs/1911.11484)]
- Content-aware Density Map for Crowd Counting and Density Estimation [[paper](https://arxiv.org/abs/1906.07258)]
- Crowd Transformer Network [[paper](https://arxiv.org/abs/1904.02774)]
- W-Net: Reinforced U-Net for Density Map Estimation [[paper](https://arxiv.org/abs/1903.11249)][[code](https://github.com/ZhengPeng7/W-Net-Keras)]![GitHub stars](https://img.shields.io/github/stars/ZhengPeng7/W-Net-Keras.svg?logo=github&label=Stars)
- Dual Path Multi-Scale Fusion Networks with Attention for Crowd Counting [[paper](https://arxiv.org/abs/1902.01115)]
- Scale-Aware Attention Network for Crowd Counting [[paper](https://arxiv.org/abs/1901.06026)]
- Crowd Counting with Density Adaption Networks [[paper](https://arxiv.org/abs/1806.10040)]
- Improving Object Counting with Heatmap Regulation [[paper](https://arxiv.org/abs/1803.05494)][[code](https://github.com/littleaich/heatmap-regulation)]![GitHub stars](https://img.shields.io/github/stars/littleaich/heatmap-regulation.svg?logo=github&label=Stars)
- Structured Inhomogeneous Density Map Learning for Crowd Counting [[paper](https://arxiv.org/abs/1801.06642)]
</details>

### 2023
### Conference
- <a name=""></a> Optimal Transport Minimization: Crowd Localization on Density Maps for Semi-Supervised Counting (**CVPR**)[[paper]()]

    #### The paper is missing. Does anyone know why?
    ***
- <a name="DGCC"></a>**[DGCC]** Domain-general Crowd Counting in Unseen Scenarios (**AAAI**)[[paper](https://arxiv.org/abs/2212.02573)] [[code](https://github.com/ZPDu/Domain-general-Crowd-Counting-in-Unseen-Scenarios)]![GitHub stars](https://img.shields.io/github/stars/ZPDu/Domain-general-Crowd-Counting-in-Unseen-Scenarios.svg?logo=github&label=Stars)

    #### Domain Generalization: proposes to use feature combination to extrat domain in-variant feature.
    ***
- <a name="SAFECount"></a>**[SAFECount]** Few-Shot Object Counting With Similarity-Aware Feature Enhancement (**WACV**)[[paper](https://arxiv.org/abs/2201.08959)] [[code](https://github.com/zhiyuanyou/SAFECount)]![GitHub stars](https://img.shields.io/github/stars/zhiyuanyou/SAFECount.svg?logo=github&label=Stars)

    #### using support image and query image to perform few-shot corwd counting 
    ***
- <a name="DMCNet"></a>**[DMCNet]** Dynamic Mixture of Counter Network for Location-Agnostic Crowd Counting (**WACV**)[[paper](https://openaccess.thecvf.com/content/WACV2023/papers/Wang_Dynamic_Mixture_of_Counter_Network_for_Location-Agnostic_Crowd_Counting_WACV_2023_paper.pdf)]

    #### local-agnostic crowd counting task: combined CNN and MLP...
    ***

### Journal
- Revisiting Crowd Counting: State-of-the-art, Trends, and Future Perspectives (**Image and Vision Computing**) [[paper](https://arxiv.org/abs/2209.07271)]

    #### A survey paper, relatively new, maybe can relief my work.
    ***
- <a name="MTCP"></a>**[MTCP]** Multi-Task Credible Pseudo-Label Learning for Semi-supervised Crowd Counting (**T-NNLS**) [[paper]()] [[code](https://github.com/ljq2000/MTCP)]![GitHub stars](https://img.shields.io/github/stars/ljq2000/MTCP.svg?logo=github&label=Stars)

    #### pseudo-label learning with multi-task: density map prediction, binary segmentation and confidence prediction. propose to using more various pseudo labeled data.
    ***
- <a name="STGN"></a>**[STGN]** Spatial-Temporal Graph Network for Video Crowd Counting (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/document/9810269)] [[code](https://github.com/wuzhe71/STGN)]![GitHub stars](https://img.shields.io/github/stars/wuzhe71/STGN.svg?logo=github&label=Stars)

    #### video crowd counting: construct spatial-temporal graph, tempora path graph, spatial pixel graph on each pyramid scale.
    ***
- <a name="CmCaF"></a>**[CmCaF]** RGB-D Crowd Counting With Cross-Modal Cycle-Attention Fusion and Fine-Coarse Supervision (**TII**) [[paper](https://ieeexplore.ieee.org/document/9765786)]

    #### RGB-D fusion method with cycle-attention fusion. It's obvious. So no more interpretation.
    ***
- <a name="STC-Crowd"></a>**[STC-Crowd]** Semi-supervised Crowd Counting with Spatial Temporal Consistency and Pseudo-label Filter (**T-CSVT**)[[paper](https://ieeexplore.ieee.org/document/10032602)]

    #### self-supervised crowd counting: utilizes spatial-temporal consistency to constrain generated pseudo density maps and uses filter to allocate weight for pseudo label. 
    ***
- <a name="LMSFFNet"></a>**[LMSFFNet]** A Lightweight Multiscale Feature Fusion Network for Remote Sensing Object Counting (**TGRS**) [[paper](https://ieeexplore.ieee.org/document/10021616)]

    #### proposes a lightweight structure to solve the multi-scale problem: a mobileViT and xxx.
    ***
- <a name="DDMD"></a>**[DDMD]** Deformable Density Estimation via Adaptive Representation (**TIP**) [[paper](https://ieeexplore.ieee.org/document/10036469)]

    #### requires bounding boxes to generate adaptive density map, constrain a new branch and utilizes dilated CNN to extract multi scale problem.
    #### obatin performance improvement on the dataset with bounding box annotations...
    ***

### 2022
### Conference
- <a name="CSS-CCNN"></a>**[CSS-CCNN]** Completely Self-Supervised Crowd Counting via Distribution Matching (**ECCV**) [[paper](https://arxiv.org/abs/2009.06420)][[code](https://github.com/val-iisc/css-ccnn)]![GitHub stars](https://img.shields.io/github/stars/val-iisc/css-ccnn.svg?logo=github&label=Stars)

    #### nature crowd follows a power law distribution and perform complertely self-supervised crowd counting...
    ***
- <a name="TSFADet"></a>**[TSFADet]** Translation, Scale and Rotation: Cross-Modal Alignment Meets RGB-Infrared Vehicle Detection (**ECCV**) [[paper](https://arxiv.org/abs/2209.13801)]

    #### multi-modal alignment in RGB-Infrared Vehicle Detection.
    #### the misalignment represent in xxx and they design a module to relief it.
    ***
- <a name="CSCA"></a>**[CSCA]** Spatio-channel Attention Blocks for Cross-modal Crowd Counting (**ACCV**) [[paper](https://arxiv.org/abs/2210.10392)] [[code](https://github.com/VCLLab/CSCA)]![GitHub stars](https://img.shields.io/github/stars/VCLLab/CSCA.svg?logo=github&label=Stars)

    #### introduces multi-modal problem in crowd counting, however, in most scenes, data with other modals are unavaliable... and spatial-channel attention emmm seems normal tec.
    ***
- <a name="CUT"></a>**[CUT]** Segmentation Assisted U-shaped Multi-scale Transformer for Crowd Counting (**BMVC**) [[paper](https://www.researchgate.net/publication/364030579_Segmentation_Assisted_U-shaped_Multi-scale_Transformer_for_Crowd_Counting)]

    #### utilizes the good performance of transformer
    #### proposes a crowd u-transformer
    #### proposes a loss function to focus more on the foreground.
    ***
- <a name="MSDTrans"></a>**[MSDTrans]** RGB-T Multi-Modal Crowd Counting Based on Transformer (**BMVC**)[[paper](https://arxiv.org/abs/2301.03033)] [[code](https://github.com/liuzywen/RGBTCC)]![GitHub stars](https://img.shields.io/github/stars/liuzywen/RGBTCC.svg?logo=github&label=Stars)

    #### perform RGB-IR crowd counting with transformer...multi-modal fusion
    ***
- <a name="LoViTCrowd"></a>**[LoViTCrowd]** Improving Local Features with Relevant Spatial Information by Vision Transformer for Crowd Counting (**BMVC**) [[paper](https://bmvc2022.mpi-inf.mpg.de/0729.pdf)] [[code](https://github.com/nguyen1312/LoViTCrowd)]![GitHub stars](https://img.shields.io/github/stars/nguyen1312/LoViTCrowd.svg?logo=github&label=Stars)

    #### an application of ViT, and then?
    ***
- <a name="SPDCN"></a>**[SPDCN]** Scale-Prior Deformable Convolution for Exemplar-Guided Class-Agnostic Counting (**BMVC**) [[paper](https://bmvc2022.mpi-inf.mpg.de/0313.pdf)]

    #### solves the scaling problem in class-agnostic counting with deformable convolution and scale-sensitive loss function.
    ***
- <a name="PAP"></a>**[PAP]** Harnessing Perceptual Adversarial Patches for Crowd Counting (**ACM CCS**) [[paper](https://arxiv.org/abs/2109.07986)]

    #### utilizes the adversarial examples to assist the model to learn scale-invariant feature.
    #### the proposed perceptual adversarial patches show good performance on adversarial learning and generalization task.
    ***
- <a name="CLTR"></a>**[CLTR]** An End-to-End Transformer Model for Crowd Localization (**ECCV**) [[paper](https://arxiv.org/abs/2202.13065)] [[code](https://github.com/dk-liang/CLTR)]![GitHub stars](https://img.shields.io/github/stars/dk-liang/CLTR.svg?logo=github&label=Stars)[[project](https://dk-liang.github.io/CLTR/)]

    #### apply set prediction paradigm for the crowd localization task with KMO based macher.
    ***
- <a name="CF-MVCC"></a>**[CF-MVCC]** Calibration-free Multi-view Crowd Counting (**ECCV**) [[paper](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136690224.pdf)]

    #### multi-view corwd counting method, waiting for supplementary...
    ***
- <a name="DC"></a>**[DC]** Discrete-Constrained Regression for Local Counting Models (**ECCV**) [[paper](https://arxiv.org/abs/2207.09865)]

    #### finds the reasons why classification methods show better performance than regression methods: inaccurate dot annotation and inappropriate gaussian kernel.
    #### futhermore, proposes a discrete regression method to avoid these problems.
    ***
- <a name="DMBA"></a>**[DMBA]** Backdoor Attacks on Crowd Counting (**ACM MM**) [[paper](https://arxiv.org/abs/2205.11398)][[code](https://github.com/Nathangitlab/Backdoor-Attacks-on-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/Nathangitlab/Backdoor-Attacks-on-Crowd-Counting.svg?logo=github&label=Stars)

    #### fine-grained counting? seems a challenaging task... counting and analyze the attributes.
    ***
- <a name="DACount"></a>**[DACount]** Semi-supervised-Crowd-Counting-via-Density-Agency (**ACM MM**) [[paper](https://arxiv.org/abs/2209.02955)][[code](https://github.com/LoraLinH/Semi-supervised-Crowd-Counting-via-Density-Agency)]![GitHub stars](https://img.shields.io/github/stars/LoraLinH/Semi-supervised-Crowd-Counting-via-Density-Agency.svg?logo=github&label=Stars)

    #### an agency-guided semi-supervised counting methods...
    ***
- <a name="ChfL"></a>**[ChfL]** Crowd Counting in the Frequency Domain (**CVPR**) [[paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Shu_Crowd_Counting_in_the_Frequency_Domain_CVPR_2022_paper.pdf)][[code](https://github.com/wbshu/Crowd_Counting_in_the_Frequency_Domain)]![GitHub stars](https://img.shields.io/github/stars/wbshu/Crowd_Counting_in_the_Frequency_Domain.svg?logo=github&label=Stars)

    #### performs crowd counting in the frequency domain
    #### proposes a loss function and prove its priority with theoretical analysis.
    ***
- <a name="GauNet"></a>**[GauNet]** Rethinking Spatial Invariance of Convolutional Networks for Object Counting (**CVPR**) [[paper](https://arxiv.org/abs/2206.05253)][[code](https://github.com/zhiqic/Rethinking-Counting)]![GitHub stars](https://img.shields.io/github/stars/zhiqic/Rethinking-Counting.svg?logo=github&label=Stars)

    #### a thinking about the spatial invariance, and a new structure to replace the tradictional convolution filter. However, it not introduced in detail in the abstract.
    #### the paper can be interpreted later.
    ***
- <a name="DR.VIC"></a>**[DR.VIC]** DR.VIC: Decomposition and Reasoning for Video Individual Counting (**CVPR**) [[paper](https://crabwq.github.io/pdf/2022%20DR.VIC.pdf)][[code](https://github.com/taohan10200/DRNet)]![GitHub stars](https://img.shields.io/github/stars/taohan10200/DRNet.svg?logo=github&label=Stars)

    #### amazing! reasoning related work! however, it is in video crowd counting
    #### reasons the pedestrain transport flow, it seem related but different to MOT.
    ***
- <a name="CDCC"></a>**[CDCC]** Leveraging Self-Supervision for Cross-Domain Crowd Counting (**CVPR**) [[paper](https://arxiv.org/abs/2103.16291)][[code](https://github.com/weizheliu/Cross-Domain-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/weizheliu/Cross-Domain-Crowd-Counting.svg?logo=github&label=Stars)

    #### training with the synthetic data and transfer the model to the real data.
    ***
- <a name="MAN"></a>**[MAN]** Boosting Crowd Counting via Multifaceted Attention (**CVPR**) [[paper](https://arxiv.org/abs/2203.02636)][[code](https://github.com/LoraLinH/Boosting-Crowd-Counting-via-Multifaceted-Attention)]![GitHub stars](https://img.shields.io/github/stars/LoraLinH/Boosting-Crowd-Counting-via-Multifaceted-Attention.svg?logo=github&label=Stars)

    #### revision in current ViT: incorporates global attention from a vanilla transformer, learnable local attention, and instance attention into the transformer. the reason for its efficiency not clear.
    ***
- <a name="BLA"></a>**[BLA]** Bi-level Alignment for Cross-Domain Crowd Counting (**CVPR**) [[paper](https://arxiv.org/abs/2205.05844)][[code](https://github.com/Yankeegsj/BLA)]![GitHub stars](https://img.shields.io/github/stars/Yankeegsj/BLA.svg?logo=github&label=Stars)

    #### bi-level alignment: task-driven data alignment, fine-grained feature alignment(foreground and background).
    #### maybe the fine-grained feature alignment can be referred.
    ***
- <a name="BMNet"></a>**[BMNet]** Represent, Compare, and Learn: A Similarity-Aware Framework for Class-Agnostic Counting (**CVPR**)[[paper](https://arxiv.org/abs/2203.08354)][[code](https://github.com/flyinglynx/Bilinear-Matching-Network)]![GitHub stars](https://img.shields.io/github/stars/flyinglynx/Bilinear-Matching-Network.svg?logo=github&label=Stars)

    #### well, class-agnostic counting is preferred to be disscussed later.
    ***
- <a name=""></a> Fine-Grained Counting with Crowd-Sourced Supervision (**CVPRW**) [[paper](https://arxiv.org/abs/2205.11398)]

    #### introduced a fine-grained counting dataset for crowd-sourced annotations.
    ***
- <a name="CrowdFormer"></a>**[CrowdFormer]** CrowdFormer: An Overlap Patching Vision Transformer for Top-Down Crowd Counting (**IJCAI**)[[paper](https://www.ijcai.org/proceedings/2022/0215.pdf)]

    #### using Patched ViT to solve the scaling problem with both the dot map and density map annotation in a top-down manner.
    ***
- <a name="WSCNN"></a>**[WSCNN]** Single Image Object Counting and Localizing using Active-Learning (**WACV**) [[paper](https://openaccess.thecvf.com/content/WACV2022/papers/Huberman-Spiegelglas_Single_Image_Object_Counting_and_Localizing_Using_Active-Learning_WACV_2022_paper.pdf)]

    #### an active learning method for object counting and localization.
    #### the definition of active learning......
    ***
- <a name="IS-Count"></a>**[IS-Count]** IS-Count: Large-Scale Object Counting from Satellite Images with Covariate-Based Importance Sampling (**AAAI**) [[paper](https://arxiv.org/abs/2112.09126)][[code](https://github.com/sustainlab-group/IS-Count)]![GitHub stars](https://img.shields.io/github/stars/sustainlab-group/IS-Count.svg?logo=github&label=Stars)

    #### emmmmm, sampling based counting, saving but the confidence is doubtful.
    ***
- <a name="STAN"></a>**[STAN]** A Spatio-Temporal Attentive Network for Video-Based Crowd Counting (**ISCC**) [[paper](https://arxiv.org/abs/2208.11339)]

    #### only illustrates that they use spatial-temporal attention to imporve counting and localization precision...
    ***
- <a name="LARL"></a>**[LARL]** Label-Aware Ranked Loss for robust People Counting using Automotive in-cabin Radar (**ICASSP**) [[paper](https://arxiv.org/abs/2110.05876v2)]

    #### design a label aware rank loss for in-cabin radar scene.
    #### since the scene is different to our requirement, skip it.
    ***
- <a name="ESA-Net"></a>**[ESA-Net]** Enhancing and Dissecting Crowd Counting By Synthetic Data (**ICASSP**) [[paper](https://arxiv.org/abs/2201.08992)]

    #### with parameterized realization, the dataset can improve the performance of many benchmark and research the influence of different factors.
    ***
- <a name="MPS"></a>**[MPS]** Multiscale Crowd Counting and Localization By Multitask Point Supervision (**ICASSP**) [[paper](https://arxiv.org/abs/2202.09942)][[code](https://github.com/RCVLab-AiimLab/crowd_counting)]![GitHub stars](https://img.shields.io/github/stars/RCVLab-AiimLab/crowd_counting.svg?logo=github&label=Stars)

    #### performs counting and localization together...then? by fusing features from multi-layer?
    ***
- <a name="TAFNet"></a>**[TAFNet]** TAFNet: A Three-Stream Adaptive Fusion Network for RGB-T Crowd Counting (**ISCAS**) [[paper](https://arxiv.org/abs/2202.08517)][[code](https://github.com/TANGHAIHAN/TAFNet)]![GitHub stars](https://img.shields.io/github/stars/TANGHAIHAN/TAFNet.svg?logo=github&label=Stars)

    #### fusion method for RGB-T images. thress-stream: RGB-T/RGB/T......
    ***
- <a name="HDNet"></a>**[HDNet]** HDNet: A Hierarchically Decoupled Network for Crowd Counting (**ICME**) [[paper](https://arxiv.org/abs/2212.05722)]

    #### decomposes the image counting task into background decomposing, foreground density decomposing, and introduces three interactions to compensate for the ignored correlation between the subtasks.
    ***
- <a name="SSDA"></a>**[SSDA]** Self-supervised Domain Adaptation in Crowd Counting (**ICIP**) [[paper](https://arxiv.org/abs/2206.03431)]

    #### introduce a domain adaptation method. unknown its priority however.
    ***
- <a name="FusionCount"></a>**[FusionCount]** FusionCount: Efficient Crowd Counting via Multiscale Feature Fusion (**ICIP**) [[paper](https://arxiv.org/abs/2202.13660)][[code](https://github.com/YimingMa/FusionCount)]![GitHub stars](https://img.shields.io/github/stars/YimingMa/FusionCount.svg?logo=github&label=Stars)

    #### fuses multi-scale feature to enlarge the receptive fields, however, I doubt the method has been proposed before.
    ***

### Journal
- <a name="MVMS"></a>**[MVMS]** Wide-Area Crowd Counting: Multi-View Fusion Networks for Counting in Large Scenes (**IJCV**) [[paper](https://arxiv.org/abs/2012.00946)](extension of [MVMS](#MVMS))

    #### maybe the first one to propose the multi-view counting task based on fusing method. not sure.
    ***
- <a name="DEFNet"></a>**[DEFNet]** DEFNet: Dual-Branch Enhanced Feature Fusion Network for RGB-T Crowd Counting (**TITS**) [[paper](https://ieeexplore.ieee.org/abstract/document/9889192)][[code](https://github.com/panyi95/DEFNet)]![GitHub stars](https://img.shields.io/github/stars/panyi95/DEFNet.svg?logo=github&label=Stars) 

    #### proposes a module to process RGB-T data......
    ***
- <a name="CLRNet"></a>**[CLRNet]** CLRNet: A Cross Locality Relation Network for Crowd Counting in Videos (**T-NNLS**) [[paper](https://ieeexplore.ieee.org/document/9913683)]
    
    #### construct location relation between frames and then? allocate different weights to different regions, like crowd and background... well illstrated but...
    ***
- <a name="AGCCM"></a>**[AGCCM]** Attention-guided Collaborative Counting (**TIP**) [[paper](https://ieeexplore.ieee.org/document/9906560)]

    #### proposed modules: Attention Guided M, Collaborative Counting M, Bi-transformer (row attention and column attention) uses different branches to collaboratively output a density map.
    ***
- <a name="GNA"></a>**[GNA]** Video Crowd Localization with Multi-focus Gaussian Neighborhood Attention and a Large-Scale Benchmark (**TMM**) [[paper](https://ieeexplore.ieee.org/document/9875106)][[code](https://github.com/HopLee6/VSCrowd-Dataset)]![GitHub stars](https://img.shields.io/github/stars/HopLee6/VSCrowd-Dataset.svg?logo=github&label=Stars) 

    #### applies a multi-focus mechanism, however, it is unclear how it works right now.
    #### furthermore, a new video counting benchmark is proposed.
    ***
- <a name="LibraNet+DQN"></a> **[LibraNet+DQN]** Counting Crowd by Weighing Counts: A Sequential Decision-Making Perspective (**T-NNLS**) [[paper](https://ieeexplore.ieee.org/document/9887967/)][[code](https://git.io/libranet)](extension of [LibraNet](#LibraNet))

    #### by applying deep reinforement learning algorithms, the methods reagrd counting as a multi-steps optimization problem...maybe...
    ***
- <a name="FIDTM"></a>**[FIDTM]** Focal Inverse Distance Transform Maps for Crowd Localization (**TMM**)[[paper](https://ieeexplore.ieee.org/document/9875106)] [[code](https://github.com/dk-liang/FIDTM)]![GitHub stars](https://img.shields.io/github/stars/dk-liang/FIDTM.svg?logo=github&label=Stars) [[project](https://dk-liang.github.io/FIDTM/)]

    #### to solve the problem in the current density map, proposes a focal inverse distance transform map and a local-maxima-detection-strategy to extract point information.
    ***
- <a name="NDConv"></a>**[NDConv]** An Improved Normed-Deformable Convolution for Crowd Counting (**SPL**) [[paper](https://arxiv.org/abs/2206.08084)]

    #### apply normalization on deformable convolution to ensure uniform sampling... nice idea, but the effect is unknown.
    ***
- <a name="RAN"></a>**[RAN]** Region-Aware Network: Model Human’s Top-Down Visual Perception Mechanism for Crowd Counting (**Neural Networks**) [[paper](https://arxiv.org/abs/2106.12163)]

    #### applies a top-down structure and tells the story well. I am not sure whether it completes the top-down structure that can allocate attention reasonably.
    ***
- <a name="HANet"></a>**[HANet]** Hybrid attention network based on progressive embedding scale-context for crowd counting (**Information Sciences**) [[paper](https://arxiv.org/abs/2106.02324)]

    #### apply paralleling spatial attention and channel attention to sovle the background noise and scaling problems simultaneously.
    ***
- <a name="TransCrowd"></a>**[TransCrowd]** TransCrowd: Weakly-Supervised Crowd Counting with Transformer (**Science China Information Sciences**) [[paper](https://arxiv.org/abs/2104.09116)] [[code](https://github.com/dk-liang/TransCrowd)]![GitHub stars](https://img.shields.io/github/stars/dk-liang/TransCrowd.svg?logo=github&label=Stars)

    #### a little bit ridiculous. using transformer to enlarge the receptive field and thought the count supervision is enough...
    #### transformer also suffer from scale variation and count is a already-tried setting... the reason why we give up it is not the receptive field.
    ***
- <a name="STNet"></a>**[STNet]** STNet: Scale Tree Network with Multi-level Auxiliator for Crowd Counting (**TMM**) [[paper](https://ieeexplore.ieee.org/document/9681311)]

    #### aiming at the scaling problem, proposes scale-tree to enhance the scale diversity and parse the scale coarse-to-fine. The auxiliator can assit feature generalization between different levels???
    ***
- <a name="SGANet"></a>**[SGANet]** Crowd Counting via Segmentation Guided Attention Networks and Curriculum Loss (**TITS**) [[paper](https://ieeexplore.ieee.org/document/9678116)]

    #### emmm, the revision is to replace vgg with inception-v3??? one more segmentation guided module and a curriculum loss are added......
    #### maybe the segmentation guided module is worth reading...
    ***
- <a name="SSR-HEF"></a>**[SSR-HEF]** SSR-HEF: Crowd Counting with Multi-Scale Semantic Refining and Hard Example Focusing (**TII**) [[paper](https://arxiv.org/abs/2204.07406)]

    #### hard example focusing and multi-scale semantic refining...
    ***
- <a name="ECCNAS"></a> **[ECCNAS]** 	ECCNAS: Efficient Crowd Counting Neural Architecture Search (**TOMM**) [[paper](https://dl.acm.org/doi/abs/10.1145/3465455)]

    #### an efficient crowd counting neural architecture search (ECCNAS) framework to search efficient crowd counting network structures
    #### copy the abstract and know that it is not what I want.
    ***
- <a name="SSCC"></a> **[SSCC]** 	Scene-specific crowd counting using synthetic training images (**Pattern Recognition**) [[paper](https://www.sciencedirect.com/science/article/pii/S0031320321006609)]

    #### the idea seems interesting, generating a synthetic scene same wih the image and leanring.
    #### therefore, we dont need the label, if not misunderstanding.
    ***
- <a name="SL-ViT"></a> **[SL-ViT]** Single-Layer Vision Transformers for More Accurate Early Exits with Less Overhead (**Neural Networks**) [[paper](https://arxiv.org/abs/2105.09121)]

    #### a combination of early exits method and ViT which can be applied in regression and classification task.
    ***
- <a name="DCST"></a> **[DCST]** Congested Crowd Instance Localization with Dilated Convolutional Swin Transformer (**Neurocomputing**) [[paper](https://arxiv.org/abs/2108.00584)]

    #### by inserting dilated convolution in different stage of ViT, the model obtains lagre receptive field and get more context information.
    ***
- A survey on deep learning-based single image crowd counting: Network design, loss function and supervisory signal (**Neurocomputing**) [[paper](https://arxiv.org/abs/2012.15685)

    #### emmmm, a survy on crowd counting, wow.
    ***

# 77 papers

### 2021
### Conference
- <a name="GNet"></a>**[GNet]** Gaussian map predictions for 3D surface feature localisation and counting (**BMVC**) [[paper](https://www.bmvc2021-virtualconference.com/assets/papers/1417.pdf)]

    #### strawberry 3D surface counting... really pratical research... however, totally different application.
    ***
- <a name="PFSNet"></a>**[PFSNet]** Robust Crowd Counting via Image Enhancement and Dynamic Feature Selection (**BMVC**) [[paper](https://www.bmvc2021-virtualconference.com/assets/papers/1387.pdf)]

    #### according to the estimated density, adjust the receptive field dynamically and adjust the images to a uniform status.
    #### it is said to outperform SASNet emmmmmmmmmmmmmmmmm. are these enough?
    ***
- <a name="URC"></a>**[URC]** Crowd Counting With Partial Annotations in an Image (**ICCV**) [[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Xu_Crowd_Counting_With_Partial_Annotations_in_an_Image_ICCV_2021_paper.pdf)]

    #### an interesting setting, with only 10% annotation, the author design a structure to learn the similarity between the regions which are annotated and not annotated.
    #### the experiments show that even with only 10% annoations, the model can keep a relatively high precision.
    ***
- <a name="MFDC"></a>**[MFDC]** Exploiting Sample Correlation for Crowd Counting With Multi-Expert Network (**ICCV**) [[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Liu_Exploiting_Sample_Correlation_for_Crowd_Counting_With_Multi-Expert_Network_ICCV_2021_paper.pdf)]

    #### proposes a method to metric data similarity to find the data to train in the expert network.
    #### applies multi-expert method for crowd counting task.
    ***
- <a name="SDNet"></a>**[SDNet]** Towards A Universal Model for Cross-Dataset Crowd Counting (**ICCV**) [[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Ma_Towards_a_Universal_Model_for_Cross-Dataset_Crowd_Counting_ICCV_2021_paper.pdf)]

    #### wishes to generate a universal model for all scenes and uses wasserstein distance based loss function to measure the scaling factor.
    ***
- <a name="P2PNet"></a>**[P2PNet]** Rethinking Counting and Localization in Crowds:A Purely Point-Based Framework (**ICCV(Oral)**) [[paper](https://arxiv.org/abs/2107.12746)][[code](https://github.com/TencentYoutuResearch/CrowdCounting-P2PNet)]![GitHub stars](https://img.shields.io/github/stars/TencentYoutuResearch/CrowdCounting-P2PNet.svg?logo=github&label=Stars)

    #### proposes a point based counting framework. maybe the first one to utilize pure point annotations.
    ***
- <a name="UEPNet"></a>**[UEPNet]** Uniformity in Heterogeneity:Diving Deep into Count Interval Partition for Crowd Counting (**ICCV**) [[paper](https://arxiv.org/abs/2107.12619)][[code](https://github.com/TencentYoutuResearch/CrowdCounting-UEPNet)]![GitHub stars](https://img.shields.io/github/stars/TencentYoutuResearch/CrowdCounting-UEPNet.svg?logo=github&label=Stars)

    #### transfer the regression problem into a classification problem by index the image part into a counting interval.
    ***
- <a name="SUA"></a>**[SUA]** Spatial Uncertainty-Aware Semi-Supervised Crowd Counting (**ICCV**) [[paper](https://arxiv.org/abs/2107.13271)][[code](https://github.com/smallmax00/SUA_crowd_counting)]![GitHub stars](https://img.shields.io/github/stars/smallmax00/SUA_crowd_counting.svg?logo=github&label=Stars)

    #### a semi-supervised method with spatial-uncertainty. its illustration is unclear.
    ***
- <a name="DKPNet"></a>**[DKPNet]** Variational Attention: Propagating Domain-Specific Knowledge for Multi-Domain Learning in Crowd Counting (**ICCV**) [[paper](https://arxiv.org/abs/2108.08023)][[code](https://github.com/Zhaoyi-Yan/DKPNet)]![GitHub stars](https://img.shields.io/github/stars/Zhaoyi-Yan/DKPNet.svg?logo=github&label=Stars)

    #### task: multi-domain learning for a generalized model.
    #### method: utilize variational attention to learn domain-specfic knowledge.
    ***
- <a name="CC-AV"></a>**[CC-AV]** Audio-Visual Transformer Based Crowd Counting (**ICCVW**) [[paper](https://arxiv.org/abs/2109.01926)]

    #### utilizes auditory information to aid visual informaton. but how and why?
    ***
- <a name="BinLoss"></a>**[BinLoss]** Wisdom of (Binned) Crowds: A Bayesian Stratification Paradigm for Crowd Counting (**ACM MM**) [[paper](https://arxiv.org/abs/2108.08784)][[code](https://github.com/atmacvit/bincrowd)]![GitHub stars](https://img.shields.io/github/stars/atmacvit/bincrowd?label=Stars&logo=Github)

    #### proposes a bayesian-based stratification method to decompose crowd counting task and a new loss function to combine MAE and MSE...
    ***
- <a name="C2MoT"></a>**[C2MoT]** Dynamic Momentum Adaptation for Zero-Shot Cross-Domain Crowd Counting (**ACM MM**) [[paper](https://dl.acm.org/doi/pdf/10.1145/3474085.3475230)][[code](https://github.com/jimmy-dq/C2MOT)]![GitHub stars](https://img.shields.io/github/stars/jimmy-dq/C2MOT?label=Stars&logo=Github)

    #### zero-shot cross-domain crowd counting, in emergency, skip.
    ***
- <a name="ASNet"></a>**[ASNet]** Coarse to Fine: Domain Adaptive Crowd Counting via Adversarial Scoring Network (**ACM MM**) [[paper](https://arxiv.org/abs/2107.12858)]

    #### domain adaptation method, skip.
    ***
- <a name="APAM"></a>**[APAM]** Towards Adversarial Patch Analysis and Certified Defense against Crowd Counting (**ACM MM**) [[paper](https://arxiv.org/abs/2104.10868)][[code](https://github.com/harrywuhust2022/Adv-Crowd-analysis)]![GitHub stars](https://img.shields.io/github/stars/harrywuhust2022/Adv-Crowd-analysis.svg?logo=github&label=Stars)

    #### an evaluation method for certified defence.
    ***
- <a name="S3"></a>**[S3]** Direct Measure Matching for Crowd Counting (**IJCAI**) [[paper](https://www.ijcai.org/proceedings/2021/0116.pdf)]

    #### directly uses point annotation to supervise the training process
    #### proposes to use sinkhorn divergence as regressive loss which is more concentrated.
    ***
- <a name="BM-Count"></a>**[BM-Count]** Bipartite Matching for Crowd Counting with Point Supervision (**IJCAI**) [[paper](https://www.ijcai.org/proceedings/2021/0119.pdf)]

    #### a bipartite matching loss and a ranking distribution learning framework to avoid the influence of density distribution.
    ***
- <a name="GLoss"></a>**[GLoss]** A Generalized Loss Function for Crowd Counting and Localization (**CVPR**) [[paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Wan_A_Generalized_Loss_Function_for_Crowd_Counting_and_Localization_CVPR_2021_paper.pdf)]

    #### proving that l2 and bayesian loss are suboptimal of transport loss.
    ***
- <a name="CVCS"></a>**[CVCS]** Cross-View Cross-Scene Multi-View Crowd Counting (**CVPR**) [[paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_Cross-View_Cross-Scene_Multi-View_Crowd_Counting_CVPR_2021_paper.pdf)]

    #### a work for multi-view crowd counting and the first one to perform cross-scene generalization.
    ***
- <a name="STANet"></a> **[STANet]** Detection, Tracking, and Counting Meets Drones in Crowds: A Benchmark (**CVPR**) [[paper](https://arxiv.org/abs/2105.02440)][[code](https://github.com/VisDrone/DroneCrowd)]![GitHub stars](https://img.shields.io/github/stars/VisDrone/DroneCrowd.svg?logo=github&label=Stars)

    #### proposes a new video counting dataset and a framework to jointly perform detection, tracking and counting.
    ***
- <a name="RGBT-CC"></a> **[RGBT-CC]** Cross-Modal Collaborative Representation Learning and a Large-Scale RGBT Benchmark for Crowd Counting (**CVPR**) [[paper](https://arxiv.org/abs/2012.04529)][[code](https://github.com/chen-judge/RGBTCrowdCounting)]![GitHub stars](https://img.shields.io/github/stars/chen-judge/RGBTCrowdCounting.svg?logo=github&label=Stars)[[Project](http://lingboliu.com/RGBT_Crowd_Counting.html#)]

    #### RGBT benchmark and a cross-modal collaborative representation learning.
    ***
- <a name="EDIREC-Net"></a> **[EDIREC-Net]** Error-Aware Density Isomorphism Reconstruction for Unsupervised Cross-Domain Crowd Counting (**AAAI**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/16245)][[code](https://github.com/GehenHe/EDIREC-Net)]![GitHub stars](https://img.shields.io/github/stars/GehenHe/EDIREC-Net.svg?logo=github&label=Stars)

    #### unsupervised domain adaptation task, skip temporarily.
    ***
- <a name="SASNet"></a> **[SASNet]** To Choose or to Fuse? Scale Selection for Crowd Counting (**AAAI**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/16360)][[code](https://github.com/TencentYoutuResearch/CrowdCounting-SASNet)]![GitHub stars](https://img.shields.io/github/stars/TencentYoutuResearch/CrowdCounting-SASNet.svg?logo=github&label=Stars)

    #### perfect idea, perfectly fit my idea. using weight patch-feature level matching to fit continuous density distribution. and utilize the idea like asnet to calculate loss function to realize multi-level optimization.
    ***
- <a name="UOT"></a> **[UOT]** Learning to Count via Unbalanced Optimal Transport (**AAAI**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/16332)]

    #### proposes to using unbalanced transport loss and present an optimization method.
    ***
- <a name="TopoCount"></a> **[TopoCount]**  Localization in the Crowd with Topological Constraints (**AAAI**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/16170)][[code](https://github.com/ShahiraAbousamra/TopoCount)]![GitHub stars](https://img.shields.io/github/stars/ShahiraAbousamra/TopoCount.svg?logo=github&label=Stars)

    #### uses topological reasoning to avoid the wrong clustered localization results.
    ***
- <a name="CFANet"></a> **[CFANet]** Coarse- and Fine-grained Attention Network with Background-aware Loss for Crowd Density Map Estimation (**WACV**) [[paper](https://arxiv.org/abs/2011.03721)][[code](https://github.com/rongliangzi/MARUNet)]![GitHub stars](https://img.shields.io/github/stars/rongliangzi/MARUNet.svg?logo=github&label=Stars)

    #### coarse-to-fine-grained attention network to focus on crowd region and background aware loss to reduce the recognition.
    ***
- <a name="BSCC"></a> **[BSCC]** Understanding the impact of mistakes on background regions in crowd counting (**WACV**) [[paper](https://arxiv.org/abs/2003.13759)]

    #### analyze the mistaken prediction on the background in depth.
    #### add a simple segementation branch to alleviate the problem
    ***
- <a name="CFOCNet"></a> **[CFOCNet]** Class-agnostic Few-shot Object Counting (**WACV**) [[paper](https://winstonhsu.info/wp-content/uploads/2020/11/yang21class-agnostic.pdf)][[code](https://github.com/SinicaGroup/Class-agnostic-Few-shot-Object-Counting)]![GitHub stars](https://img.shields.io/github/stars/SinicaGroup/Class-agnostic-Few-shot-Object-Counting.svg?logo=github&label=Stars)

    #### maybe the first one (new bing proved) proposes the new task::::::::::
    ***
- <a name="SCALNet"></a> **[SCALNet]** Dense Point Prediction: A Simple Baseline for Crowd Counting and Localization (**ICMEW**) [[paper](https://arxiv.org/abs/2104.12505)][[code](https://github.com/WangyiNTU/SCALNet)]![GitHub stars](https://img.shields.io/github/stars/WangyiNTU/SCALNet.svg?logo=github&label=Stars)

    #### an end-to-end framework to handle counting and localization tasks with novel loss function.
    ***
- <a name="DSNet"></a> **[DSNet]** Dense Scale Network for Crowd Counting (**ICMR**) [[paper](https://arxiv.org/abs/1906.09707)][unofficial code: [PyTorch](https://github.com/rongliangzi/Dense-Scale-Network-for-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/rongliangzi/Dense-Scale-Network-for-Crowd-Counting.svg?logo=github&label=Stars)

    #### emmmm, using dilated Conv with dense block. maybe. it is intuitive but not novel.
    ***
- <a name="FCVF"></a> **[FCVF]** Learning Factorized Cross-View Fusion for Multi-View Crowd Counting (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9428284)]

    #### as its title, cross-view fusion for multi-view counting.
    ***
- <a name="IDK"></a> **[IDK]** Leveraging Intra-Domain Knowledge to Strengthen Cross-Domain Crowd Counting (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9428159)]

    #### for cross-domain counting, leverage in-domain knowledge (from synthetic data). skip and no more details temporarily.
    ***
- <a name="CRANet"></a> **[CRANet]** CRANet: Cascade Residual Attention Network for Crowd Counting (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9428236)]

    #### proposes cascade residual attentoin to filter background noise.
    ***

# above all, about 109 papers

### Journal
- <a name="DPDNet"></a>**[DPDNet]** Locating and Counting Heads in Crowds With a Depth Prior (**T-PAMI**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9601215)] [[code](https://github.com/svip-lab/Locating_Counting_with_a_Depth_Prior)]![GitHub stars](https://img.shields.io/github/stars/svip-lab/Locating_Counting_with_a_Depth_Prior.svg?logo=github&label=Stars)

    #### using RGB-D data, skip.
    ***
- <a name="EPF"></a>**[EPF]** Counting People by Estimating People Flows (**TPAMI**) [[paper](https://arxiv.org/abs/2012.00452)][[code](https://github.com/weizheliu/People-Flows)]![GitHub stars](https://img.shields.io/github/stars/weizheliu/People-Flows.svg?logo=github&label=Stars)

    #### utilize people flow in video sequences. skip.
    ***
- <a name="LA-Batch"></a>**[LA-Batch]** Locality-Aware Crowd Counting (**TPAMI**) [[paper](https://www.computer.org/csdl/journal/tp/5555/01/09346018/1qV39sNsjWU)]

    #### proposes two seperated modules to divide image patches and perform data augmentation according to loss.
    ***
- <a name="AutoScale"></a>**[AutoScale]** AutoScale: Learning to Scale for Crowd Counting (**IJCV**) [[paper](https://link.springer.com/article/10.1007/s11263-021-01542-z)] (extension of [L2SM](#L2SM))[[code](https://github.com/dk-liang/AutoScale)]![GitHub stars](https://img.shields.io/github/stars/dk-liang/AutoScale.svg?logo=github&label=Stars)

    #### learn to scale, seperate the overlapped blob. alleviate the problem in density map.
    ***
- <a name="DSACA"></a>**[DSACA]** Dilated-Scale-Aware Attention ConvNet For Multi-Class Object Counting  (**SPL**) [[paper](https://ieeexplore.ieee.org/abstract/document/9479708)] [[code](https://github.com/PRIS-CV/DSACA)]![GitHub stars](https://img.shields.io/github/stars/PRIS-CV/DSACA.svg?logo=github&label=Stars)

    #### emmm, multi-object counting with dilated convolution and etc.
    ***
- <a name="NLT"></a> **[NLT]** Neuron Linear Transformation: Modeling the Domain Shift for Crowd Counting (**T-NNLS**) [[paper](https://arxiv.org/abs/2004.02133)] [[code]](https://github.com/taohan10200/NLT)]![GitHub stars](https://img.shields.io/github/stars/taohan10200/NLT.svg?logo=github&label=Stars)

    #### domain shift for crowd counting. skip it. 
    ***
- <a name="DACC"></a> **[DACC]** Domain-Adaptive Crowd Counting via High-Quality Image Translation and Density Reconstruction (**T-NNLS**) [[paper](https://arxiv.org/abs/1912.03677)]

    #### domain adaptation. skip.
    ***
- <a name="MATT"></a> **[MATT]** Towards Using Count-level Weak Supervision for Crowd Counting (**Pattern Recognition**) [[paper](https://arxiv.org/abs/2003.00164)]

    #### count-level weak supervision for counting. small amount position annotation and large amount number annotation.
    ***
- <a name="D2C"></a> **[D2C]** Decoupled Two-Stage Crowd Counting and Beyond (**TIP**) [[paper](https://ieeexplore.ieee.org/document/9347700)][[code](https://github.com/hustaia/Decoupled_Two-Stage_Counting)]![GitHub stars](https://img.shields.io/github/stars/hustaia/Decoupled_Two-stage_Counting.svg?logo=github&label=Stars)

    #### decouple the counting task into two stage, probability map estimation (can be called foreground/background segment maybe) and counting number estimation. the countor can learn from synthetic data.
    ***
- <a name="TBC"></a> **[TBC]** Tracking-by-Counting: Using Network Flows on Crowd Density Maps for Tracking Multiple Targets (**TIP**) [[paper](https://ieeexplore.ieee.org/document/9298464)]

    #### counting for tracking... skip
    ***
- <a name="FGCC"></a> **[FGCC]** Fine-Grained Crowd Counting (**TIP**) [[paper](https://arxiv.org/abs/2007.06146)]

    #### fine-grained counting more than counting... attirbutes.
    ***
- <a name="PSODC"></a> **[PSODC]** A Self-Training Approach for Point-Supervised Object Detection and Counting in Crowds (**TIP**) [[paper](https://arxiv.org/abs/2007.12831)][[code](https://github.com/WangyiNTU/Point-supervised-crowd-detection)]![GitHub stars](https://img.shields.io/github/stars/WangyiNTU/Point-supervised-crowd-detection.svg?logo=github&label=Stars)

    #### a self-training method for object detection and crwod counting with point annotations.
    ***
- <a name="EPA"></a> **[EPA]** Embedding Perspective Analysis Into Multi-Column Convolutional Neural Network for Crowd Counting (**TIP**) [[paper](https://ieeexplore.ieee.org/document/9293174)]

    #### analyzes the perspective embedding and group the scene to solve the scaling problem.
    ***
- <a name="PFDNet"></a>**[PFDNet]** Crowd Counting via Perspective-Guided Fractional-Dilation Convolution (**TMM**) [[paper](https://ieeexplore.ieee.org/document/9468694)](extension of [PGCNet](#PGCNet))

    #### focuses on fractional-dilation, the specific implementation is unknown.
    ***
- <a name="STDNet"></a> **[STDNet]** Spatiotemporal Dilated Convolution with Uncertain Matching for Video-based Crowd Estimation (**TMM**) [[paper](https://arxiv.org/abs/2101.12439)]

    #### counting for video. decomposition of 3D convolution and the application of dilated convolution.
    ***
- <a name="AdaCrowd"></a> **[AdaCrowd]** AdaCrowd: Unlabeled Scene Adaptation for Crowd Counting (**TMM**) [[paper](https://arxiv.org/abs/2010.12141)][[code](https://github.com/maheshkkumar/adacrowd)]![GitHub stars](https://img.shields.io/github/stars/maheshkkumar/adacrowd.svg?logo=github&label=Stars)

    #### scene adptation with unlabel data. focus on a specific scene.
    ***
- <a name="DCANet"></a>**[DCANet]** Towards Learning Multi-domain Crowd Counting (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9658506)] [[code](https://github.com/Zhaoyi-Yan/DCANet)]![GitHub stars](https://img.shields.io/github/stars/Zhaoyi-Yan/DCANet.svg?logo=github&label=Stars)

    #### using one model to adapt to multi-domain.
    ***
- <a name="PDANet"></a> **[PDANet]** PDANet: Pyramid Density-aware Attention Net for Accurate Crowd Counting (**Neurocomputing**) [[paper](https://arxiv.org/abs/2001.05643)]

    #### pyramid structure for multi-scale and density-aware decoder to divide density level. at last, sum up with attention.
    ***
- <a name="ScSiNet"></a> **[ScSiNet]** Interlayer and Intralayer Scale Aggregation for Scale-invariant Crowd Counting (**Neurocomputing**) [[paper](https://arxiv.org/abs/2005.11943)]

    #### try to extract scale-invariant feature with specific transformation. propose a randomly intergrated loss to fit the density shift.
    ***
- <a name="PRM"></a> **[PRM]** Towards More Effective PRM-based Crowd Counting via A Multi-resolution Fusion and Attention Network (**Neurocomputing**) [[paper](https://arxiv.org/abs/2112.09664)]

    #### fuse multi-resolution feature and utilize orginal feature to extract foreground to fusion.......
    ***
- <a name="DeepCorn"></a> **[DeepCorn]** DeepCorn: A Semi-Supervised Deep Learning Method for High-Throughput Image-Based Corn Kernel Counting and Yield Estimation (**Knowledge-Based Systems**) [[paper](https://arxiv.org/abs/2007.10521)]

    #### emmm special field.... maybe i can read it later......... corn... remind me of......
    ***
# sum up to 130 papers
#### now let classify them.

### 2020
### Conference
- <a name="DM-Count"></a> **[DM-Count]** Distribution Matching for Crowd Counting (**NeurIPS**) [[paper](https://arxiv.org/abs/2009.13077)][[code](https://github.com/cvlab-stonybrook/DM-Count)]![GitHub stars](https://img.shields.io/github/stars/cvlab-stonybrook/DM-Count.svg?logo=github&label=Stars)
- <a name="MNA"></a> **[MNA]** Modeling Noisy Annotations for Crowd Counting (**NeurIPS**) [[paper](http://visal.cs.cityu.edu.hk/static/pubs/conf/nips2020-noisycc-web.pdf)]
- <a name="SKT"></a> **[SKT]** Efficient Crowd Counting via Structured Knowledge Transfer (**ACM MM(oral)**) [[paper](https://arxiv.org/abs/2003.10120)][[code](https://github.com/HCPLab-SYSU/SKT)]![GitHub stars](https://img.shields.io/github/stars/HCPLab-SYSU/SKT.svg?logo=github&label=Stars)
- <a name="DPN"></a> **[DPN]** Learning Scales from Points: A Scale-aware Probabilistic Model for Crowd Counting (**ACM MM(oral)**) [[paper](https://dl.acm.org/doi/10.1145/3394171.3413642)]
- <a name="RDBT"></a> **[RDBT]** Towards Unsupervised Crowd Counting via Regression-Detection Bi-knowledge Transfer (**ACM MM**) [[paper](https://arxiv.org/abs/2008.05383)]
- <a name="VisDrone-CC2020"></a> **[VisDrone-CC2020]** VisDrone-CC2020: The Vision Meets Drone Crowd Counting Challenge Results (**ECCV**) [[paper](https://arxiv.org/abs/2107.08766)]
- <a name="EPF"></a> **[EPF]** Estimating People Flows to Better Count Them in Crowded Scenes (**ECCV**) [[paper](https://arxiv.org/abs/1911.10782)][[code](https://github.com/weizheliu/People-Flows)]![GitHub stars](https://img.shields.io/github/stars/weizheliu/People-Flows.svg?logo=github&label=Stars)
- <a name="AMSNet"></a> **[AMSNet]** NAS-Count: Counting-by-Density with Neural Architecture Search (**ECCV**) [[paper](https://arxiv.org/abs/2003.00217)]
- <a name="AMRNet"></a> **[AMRNet]** Adaptive Mixture Regression Network with Local Counting Map for Crowd Counting (**ECCV**) [[paper](https://arxiv.org/abs/2005.05776)][[code](https://github.com/xiyang1012/Local-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/xiyang1012/Local-Crowd-Counting.svg?logo=github&label=Stars)
- <a name="LibraNet"></a> **[LibraNet]** Weighting Counts: Sequential Crowd Counting by Reinforcement Learning (**ECCV**) [[paper](https://arxiv.org/abs/2007.08260)][[code](https://github.com/poppinace/libranet)]![GitHub stars](https://img.shields.io/github/stars/poppinace/libranet.svg?logo=github&label=Stars)
- <a name="GP"></a> **[GP]** Learning to Count in the Crowd from Limited Labeled Data (**ECCV**) [[paper](https://arxiv.org/abs/2007.03195)]
- <a name="IRAST"></a> **[IRAST]** Semi-supervised Crowd Counting via Self-training on Surrogate Tasks (**ECCV**) [[paper](https://arxiv.org/abs/2007.03207)]
- <a name="PSSW"></a> **[PSSW]** Active Crowd Counting with Limited Supervision (**ECCV**) [[paper](https://arxiv.org/abs/2007.06334)]
- <a name="CCLS"></a> **[CCLS]** Weakly-Supervised Crowd Counting Learns from Sorting rather than Locations (**ECCV**) [[paper](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123530001.pdf)]
- <a name="Bi-pathNet"></a> **[Bi-pathNet]** A Flow Base Bi-path Network for Cross-scene Video Crowd Understanding in Aerial View (**ECCVW**) [[paper](https://arxiv.org/abs/2009.13723)]
- <a name="ADSCNet"></a> **[ADSCNet]** Adaptive Dilated Network with Self-Correction Supervision for Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Bai_Adaptive_Dilated_Network_With_Self-Correction_Supervision_for_Counting_CVPR_2020_paper.pdf)] 
- <a name="RPNet"></a> **[RPNet]** Reverse Perspective Network for Perspective-Aware Object Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_Reverse_Perspective_Network_for_Perspective-Aware_Object_Counting_CVPR_2020_paper.pdf)] [[code](https://github.com/CrowdCounting)]
- <a name="ASNet"></a> **[ASNet]** Attention Scaling for Crowd Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Jiang_Attention_Scaling_for_Crowd_Counting_CVPR_2020_paper.pdf)] [[code](https://github.com/laridzhang/ASNet)]![GitHub stars](https://img.shields.io/github/stars/laridzhang/ASNet.svg?logo=github&label=Stars)
- <a name="SRF-Net"></a> **[SRF-Net]** Scale-Aware Rolling Fusion Network for Crowd Counting (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9102854)]
- <a name="EDC"></a> **[EDC]** Learning Error-Driven Curriculum for Crowd Counting (**ICPR**) [[paper](https://arxiv.org/pdf/2007.09676.pdf)][[code](https://github.com/FDU-VTS/TutorNet_Crowd_Counting)]![GitHub stars](https://img.shields.io/github/stars/FDU-VTS/TutorNet_Crowd_Counting.svg?logo=github&label=Stars)
- <a name="PRM"></a> **[PRM]** Multi-Resolution Fusion and Multi-scale Input Priors Based Crowd Counting (**ICPR**) [[paper](https://arxiv.org/abs/2010.01664)]
- <a name="M-SFANet"></a> **[M-SFANet]** Encoder-Decoder Based Convolutional Neural Networks with Multi-Scale-Aware Modules for Crowd Counting (**ICPR**) [[paper](https://arxiv.org/abs/2003.05586)][[code](https://github.com/Pongpisit-Thanasutives/Variations-of-SFANet-for-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/Pongpisit-Thanasutives/Variations-of-SFANet-for-Crowd-Counting.svg?logo=github&label=Stars)
- <a name="HSRNet"></a> **[HSRNet]** Crowd Counting via Hierarchical Scale Recalibration Network (**ECAI**) [[paper](https://arxiv.org/abs/2003.03545)]
- <a name="DeepCount"></a> **[DeepCount]** Deep Density-aware Count Regressor (**ECAI**) [[paper](https://arxiv.org/abs/1908.03314)][[code](https://github.com/GeorgeChenZJ/deepcount)]![GitHub stars](https://img.shields.io/github/stars/GeorgeChenZJ/deepcount.svg?logo=github&label=Stars)
- <a name="SOFA-Net"></a> **[SOFA-Net]** SOFA-Net: Second-Order and First-order Attention Network for Crowd Counting (**BMVC**) [[paper](https://arxiv.org/abs/2008.03723)]
- <a name="CWAN"></a> **[CWAN]** Weakly Supervised Crowd-Wise Attention For Robust Crowd Counting (**ICASSP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9054258)]
- <a name="AGRD"></a> **[AGRD]** Attention Guided Region Division for Crowd Counting (**ICASSP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9053761)]
- <a name="BBA-NET"></a> **[BBA-NET]** BBA-NET: A Bi-Branch Attention Network For Crowd Counting (**ICASSP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9053955)]
- <a name="SMANet"></a> **[SMANet]** Stochastic Multi-Scale Aggregation Network for Crowd Counting (**ICASSP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9054238)]
- <a name="Stacked-Pool"></a> **[Stacked-Pool]** Stacked Pooling For Boosting Scale Invariance Of Crowd Counting (**ICASSP**) [[paper](https://siyuhuang.github.io/papers/ICASSP-2020-STACKED%20POOLING%20FOR%20BOOSTING%20SCALE%20INVARIANCE%20OF%20CROWD%20COUNTING.pdf)] [[arxiv](https://arxiv.org/abs/1808.07456)] [[code](http://github.com/siyuhuang/crowdcount-stackpool)]![GitHub stars](https://img.shields.io/github/stars/siyuhuang/crowdcount-stackpool.svg?logo=github&label=Stars)
- <a name="MSPNET"></a> **[MSPNET]** Multi-supervised Parallel Network for Crowd Counting (**ICASSP**) [[paper](https://crabwq.github.io/pdf/2020%20MSPNET%20Multi-supervised%20Parallel%20Network%20for%20Crowd%20Counting.pdf)]
- <a name="ASPDNet"></a> **[ASPDNet]** Counting dense objects in remote sensing images (**ICASSP**) [[paper](https://arxiv.org/abs/2002.05928)]
- <a name="FSC"></a> **[FSC]** Focus on Semantic Consistency for Cross-domain Crowd Understanding (**ICASSP**) [[paper](https://arxiv.org/abs/2002.08623)]
- <a name="C-CNN"></a> **[C-CNN]** A Real-Time Deep Network for Crowd Counting (**ICASSP**) [[arxiv](https://arxiv.org/abs/2002.06515)][[ieee](https://ieeexplore.ieee.org/abstract/document/9053780/)]
- <a name="HyGnn"></a> **[HyGnn]** Hybrid  Graph  Neural  Networks  for  Crowd  Counting (**AAAI**) [[paper](https://arxiv.org/abs/2002.00092)]
- <a name="DUBNet"></a> **[DUBNet]** Crowd Counting with Decomposed Uncertainty (**AAAI**) [[paper](https://arxiv.org/abs/1903.07427)]
- <a name="SDANet"></a> **[SDANet]** Shallow  Feature  based  Dense  Attention  Network  for  Crowd  Counting (**AAAI**) [[paper](http://wrap.warwick.ac.uk/130173/1/WRAP-shallow-feature-dense-attention-crowd-counting-Han-2019.pdf)]
- <a name="3DCC"></a> **[3DCC]** 3D Crowd Counting via Multi-View Fusion with 3D Gaussian Kernels (**AAAI**) [[paper](https://arxiv.org/abs/2003.08162)][[Project](http://visal.cs.cityu.edu.hk/research/aaai20-3d-counting/)]
- <a name="FFSA"></a> **[FSSA]** Few-Shot Scene Adaptive Crowd Counting Using Meta-Learning (**WACV**) [[paper](https://arxiv.org/abs/2002.00264)][[code](https://github.com/maheshkkumar/fscc)] ![GitHub stars](https://img.shields.io/github/stars/maheshkkumar/fscc.svg?logo=github&label=Stars)
- <a name="CC-Mod"></a> **[CC-Mod]** Plug-and-Play Rescaling Based Crowd Counting in Static Images (**WACV**) [[paper](https://arxiv.org/abs/2001.01786)]
- <a name="CTN"></a> **[CTN]** Uncertainty Estimation and Sample Selection for Crowd Counting (**ACCV**) [[paper](https://arxiv.org/abs/2009.14411)]
- <a name="ikNN"></a> **[ikNN]** Improving Dense Crowd Counting Convolutional Neural Networks using Inverse k-Nearest Neighbor Maps and Multiscale Upsampling (**VISAPP**) [[paper](https://arxiv.org/abs/1902.05379)]

### Journal
- <a name="NWPU"></a> **[NWPU]** NWPU-Crowd: A Large-Scale Benchmark for Crowd Counting and Localization (**T-PAMI**) [[paper](https://arxiv.org/abs/2001.03360)][[code](https://gjy3035.github.io/NWPU-Crowd-Sample-Code/)]![GitHub stars](https://img.shields.io/github/stars/gjy3035/NWPU-Crowd-Sample-Code.svg?logo=github&label=Stars)
- <a name="KDMG"></a> **[KDMG]** Kernel-based Density Map Generation for Dense Object Counting (**T-PAMI**) [[paper](https://ieeexplore.ieee.org/document/9189836)][[code](https://github.com/jia-wan/KDMG_Counting)]![GitHub stars](https://img.shields.io/github/stars/jia-wan/KDMG_Counting.svg?logo=github&label=Stars)
- <a name="JHU-CROWD"></a> **[JHU-CROWD]** JHU-CROWD++: Large-Scale Crowd Counting Dataset and A Benchmark Method (**T-PAMI**) [[paper](https://arxiv.org/abs/2004.03597)](extension of [CG-DRCN](#CG-DRCN))
- <a name="LSC-CNN"></a> **[LSC-CNN]** Locate, Size and Count: Accurately Resolving People in Dense Crowds via Detection (**T-PAMI**) [[paper](https://arxiv.org/abs/1906.07538)][[code](https://github.com/val-iisc/lsc-cnn)]![GitHub stars](https://img.shields.io/github/stars/val-iisc/lsc-cnn.svg?logo=github&label=Stars)
- <a name="PWCU"></a> **[PWCU]** Pixel-wise Crowd Understanding via Synthetic Data (**IJCV**) [[paper](https://arxiv.org/abs/2007.16032)]![GitHub stars](https://img.shields.io/github/stars/gjy3035/GCC-SFCN.svg?logo=github&label=Stars)
- <a name="CRNet"></a> **[CRNet]** Crowd Counting via Cross-stage Refinement Networks (**TIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9096602)][[code](https://github.com/lytgftyf/Crowd-Counting-via-Cross-stage-Refinement-Networks)] ![GitHub stars](https://img.shields.io/github/stars/lytgftyf/Crowd-Counting-via-Cross-stage-Refinement-Networks.svg?logo=github&label=Stars)
- <a name="BNFDD"></a> **[BNFDD]** Background Noise Filtering and Distribution Dividing for Crowd Counting (**TIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9161353)]
- <a name="FADA"></a> **[FADA]** Feature-aware Adaptation and Density Alignment for Crowd Counting in Video Surveillance (**TCYB**) [[paper](https://arxiv.org/abs/1912.03672)]
- <a name="MS-GAN"></a> **[MS-GAN]** Adversarial Learning for Multiscale Crowd Counting Under Complex Scenes (**TCYB**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8949751)]
- <a name="DCL"></a> **[DCL]** Density-aware Curriculum Learning for Crowd Counting (**TCYB**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9275392)][[code](https://github.com/Elin24/DCL-CrowdCounting)]![GitHub stars](https://img.shields.io/github/stars/Elin24/DCL-CrowdCounting.svg?logo=github&label=Stars)
- <a name="ZoomCount"></a> **[ZoomCount]** ZoomCount: A Zooming Mechanism for Crowd Counting in Static Images (**T-CSVT**) [[paper](https://arxiv.org/abs/2002.12256)]
- <a name="DensityCNN"></a> **[DensityCNN]** Density-Aware Multi-Task Learning for Crowd Counting (**TMM**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9037113)]
- <a name="DENet"></a> **[DENet]** DENet: A Universal Network for Counting Crowd with Varying Densities and Scales (**TMM**) [[paper](https://arxiv.org/abs/1904.08056)][[code](https://github.com/liuleiBUAA/DENet)]![GitHub stars](https://img.shields.io/github/stars/liuleiBUAA/DENet.svg?logo=github&label=Stars)
- <a name="CLPNet"></a> **[CLPNet]** Cross-Level Parallel Network for Crowd Counting (**TII**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8798674)]
- <a name="FMLF"></a> **[FMLF]** Crowd Density Estimation Using Fusion of Multi-Layer Features (**TITS**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9063540)]
- <a name="MLSTN"></a> **[MLSTN]** Multi-level feature fusion based Locality-Constrained Spatial Transformer network for video crowd counting (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231220301454)](extension of [LSTN](#LSTN))
- <a name="SRN+PS"></a> **[SRN+PS]** Scale-Recursive Network with point supervision for crowd scene analysis (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231219317795)]
- <a name="ASDF"></a> **[ASDF]** Counting crowds with varying densities via adaptive scenario discovery framework (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231220302356)](extension of [ASD](#ASD))
- <a name="CAT-CNN"></a> **[CAT-CNN]** Crowd counting with crowd attention convolutional neural network (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231219316662)]
- <a name="RRP"></a> **[RRP]** Relevant Region Prediction for Crowd Counting (**Neurocomputing**) [[paper](https://arxiv.org/abs/2005.09816)]
- <a name="SCAN"></a> **[SCAN]** Crowd Counting via Scale-Communicative Aggregation Networks (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231220308778)](extension of [MVSAN](#MVSAN))
- <a name="MobileCount"></a> **[MobileCount]** MobileCount: An Efficient Encoder-Decoder Framework for Real-Time Crowd Counting (**Neurocomputing**) [[conference paper](https://link.springer.com/chapter/10.1007/978-3-030-31723-2_50)] [[journal paper](https://www.sciencedirect.com/science/article/pii/S0925231220308912)] [[code](https://github.com/SelinaFelton/MobileCount)]![GitHub stars](https://img.shields.io/github/stars/SelinaFelton/MobileCount.svg?logo=github&label=Stars)
- <a name="TAN"></a> **[TAN]** Fast Video Crowd Counting with a Temporal Aware Network (**Neurocomputing**) [[paper](https://arxiv.org/abs/1907.02198)]
- <a name="CFANet"></a> **[MH-METRONET]** MH-MetroNet—A Multi-Head CNN for Passenger-Crowd Attendance Estimation (**JImaging**) [[paper](https://www.mdpi.com/759202)][[code]( https://bitbucket.org/isasi-lecce/mh-metronet/src/master/)]

### 2019
### Conference
- <a name="CG-DRCN"></a> **[CG-DRCN]** Pushing the Frontiers of Unconstrained Crowd Counting: New Dataset and Benchmark Method (**ICCV**)[[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sindagi_Pushing_the_Frontiers_of_Unconstrained_Crowd_Counting_New_Dataset_and_ICCV_2019_paper.pdf)]
- <a name="ADMG"></a> **[ADMG]** Adaptive Density Map Generation for Crowd Counting (**ICCV**)[[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wan_Adaptive_Density_Map_Generation_for_Crowd_Counting_ICCV_2019_paper.pdf)]
- <a name="DSSINet"></a> **[DSSINet]** Crowd Counting with Deep Structured Scale Integration Network (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_Crowd_Counting_With_Deep_Structured_Scale_Integration_Network_ICCV_2019_paper.pdf)][[code](https://github.com/Legion56/Counting-ICCV-DSSINet)] ![GitHub stars](https://img.shields.io/github/stars/Legion56/Counting-ICCV-DSSINet.svg?logo=github&label=Stars)
- <a name="RANet"></a> **[RANet]** Relational Attention Network for Crowd Counting (**ICCV**)[[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhang_Relational_Attention_Network_for_Crowd_Counting_ICCV_2019_paper.pdf)]
- <a name="ANF"></a> **[ANF]** Attentional Neural Fields for Crowd Counting (**ICCV**)[[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhang_Attentional_Neural_Fields_for_Crowd_Counting_ICCV_2019_paper.pdf)]
- <a name="SPANet"></a> **[SPANet]** Learning Spatial Awareness to Improve Crowd Counting (**ICCV(oral)**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Cheng_Learning_Spatial_Awareness_to_Improve_Crowd_Counting_ICCV_2019_paper.pdf)]
- <a name="MBTTBF"></a> **[MBTTBF]** Multi-Level Bottom-Top and Top-Bottom Feature Fusion for Crowd Counting (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sindagi_Multi-Level_Bottom-Top_and_Top-Bottom_Feature_Fusion_for_Crowd_Counting_ICCV_2019_paper.pdf)]
- <a name="CFF"></a> **[CFF]** Counting with Focus for Free (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Shi_Counting_With_Focus_for_Free_ICCV_2019_paper.pdf)][[code](https://github.com/shizenglin/Counting-with-Focus-for-Free)] ![GitHub stars](https://img.shields.io/github/stars/shizenglin/Counting-with-Focus-for-Free.svg?logo=github&label=Stars)
- <a name="L2SM"></a> **[L2SM]** Learn to Scale: Generating Multipolar Normalized Density Map for Crowd Counting (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Xu_Learn_to_Scale_Generating_Multipolar_Normalized_Density_Maps_for_Crowd_ICCV_2019_paper.pdf)]
- <a name="S-DCNet"></a> **[S-DCNet]** From Open Set to Closed Set: Counting Objects by Spatial Divide-and-Conquer (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Xiong_From_Open_Set_to_Closed_Set_Counting_Objects_by_Spatial_ICCV_2019_paper.pdf)][[code](https://github.com/xhp-hust-2018-2011/S-DCNet)]![GitHub stars](https://img.shields.io/github/stars/xhp-hust-2018-2011/S-DCNet.svg?logo=github&label=Stars)
- <a name="BL"></a> **[BL]** Bayesian Loss for Crowd Count Estimation with Point Supervision (**ICCV(oral)**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Ma_Bayesian_Loss_for_Crowd_Count_Estimation_With_Point_Supervision_ICCV_2019_paper.pdf)][[code](https://github.com/ZhihengCV/Bayesian-Crowd-Counting)] ![GitHub stars](https://img.shields.io/github/stars/ZhihengCV/Bayesian-Crowd-Counting.svg?logo=github&label=Stars)
- <a name="PGCNet"></a> **[PGCNet]** Perspective-Guided Convolution Networks for Crowd Counting (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Yan_Perspective-Guided_Convolution_Networks_for_Crowd_Counting_ICCV_2019_paper.pdf)][[code](https://github.com/Zhaoyi-Yan/PGCNet)]![GitHub stars](https://img.shields.io/github/stars/Zhaoyi-Yan/PGCNet.svg?logo=github&label=Stars)
- <a name="SACANet"></a> **[SACANet]** Crowd Counting on Images with Scale Variation and Isolated Clusters (**ICCVW**) [[paper](https://arxiv.org/abs/1909.03839)]
- <a name="McML"></a> **[McML]** Improving the Learning of Multi-column Convolutional Neural Network for Crowd Counting (**ACM MM**) [[paper](https://dl.acm.org/citation.cfm?doid=3343031.3350898)]
- <a name="DADNet"></a> **[DADNet]** DADNet: Dilated-Attention-Deformable ConvNet for Crowd Counting (**ACM MM**) [[paper](https://dl.acm.org/citation.cfm?doid=3343031.3350881)] 
- <a name="MRNet"></a> **[MRNet]** Crowd Counting via Multi-layer Regression (**ACM MM**) [[paper](https://dl.acm.org/citation.cfm?doid=3343031.3350914)]
- <a name="MRCNet"></a> **[MRCNet]** MRCNet: Crowd Counting and Density Map Estimation in Aerial and Ground Imagery (**BMVCW**)[[paper](https://arxiv.org/abs/1909.12743)]
- <a name="E3D"></a> **[E3D]** Enhanced 3D convolutional networks for crowd counting (**BMVC**) [[paper](https://arxiv.org/abs/1908.04121)]
- <a name="OSSS"></a> **[OSSS]** One-Shot Scene-Specific Crowd Counting (**BMVC**) [[paper](https://bmvc2019.org/wp-content/uploads/papers/0209-paper.pdf)]
- <a name="RAZ-Net"></a> **[RAZ-Net]** Recurrent Attentive Zooming for Joint Crowd Counting and Precise Localization (**CVPR**) [[paper](http://www.muyadong.com/paper/cvpr19_0484.pdf)]
- <a name="RDNet"></a> **[RDNet]** Density Map Regression Guided Detection Network for RGB-D Crowd Counting and Localization (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Lian_Density_Map_Regression_Guided_Detection_Network_for_RGB-D_Crowd_Counting_CVPR_2019_paper.pdf)][[code](https://github.com/svip-lab/RGBD-Counting)] ![GitHub stars](https://img.shields.io/github/stars/svip-lab/RGBD-Counting.svg?logo=github&label=Stars)
- <a name="RRSP"></a> **[RRSP]** Residual Regression with Semantic Prior for Crowd Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wan_Residual_Regression_With_Semantic_Prior_for_Crowd_Counting_CVPR_2019_paper.pdf)][[code](https://github.com/jia-wan/ResidualRegression-pytorch)] ![GitHub stars](https://img.shields.io/github/stars/jia-wan/ResidualRegression-pytorch.svg?logo=github&label=Stars)
- <a name="MVMS"></a> **[MVMS]** Wide-Area Crowd Counting via Ground-Plane Density Maps and Multi-View Fusion CNNs (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Wide-Area_Crowd_Counting_via_Ground-Plane_Density_Maps_and_Multi-View_Fusion_CVPR_2019_paper.pdf)] [[Project](http://visal.cs.cityu.edu.hk/research/cvpr2019wacc/)] [[Dataset&Code](http://visal.cs.cityu.edu.hk/research/citystreet/)]
- <a name="AT-CFCN"></a> **[AT-CFCN]** Leveraging Heterogeneous Auxiliary Tasks to Assist Crowd Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhao_Leveraging_Heterogeneous_Auxiliary_Tasks_to_Assist_Crowd_Counting_CVPR_2019_paper.pdf)]
- <a name="TEDnet"></a> **[TEDnet]** Crowd Counting and Density Estimation by Trellis Encoder-Decoder Networks (**CVPR**) [[paper](https://arxiv.org/abs/1903.00853)]
- <a name="CAN"></a> **[CAN]** Context-Aware Crowd Counting (**CVPR**) [[paper](https://arxiv.org/pdf/1811.10452.pdf)] [[code](https://github.com/weizheliu/Context-Aware-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/weizheliu/Context-Aware-Crowd-Counting.svg?logo=github&label=Stars)
- <a name="PACNN"></a> **[PACNN]** Revisiting Perspective Information for Efficient Crowd Counting (**CVPR**)[[paper](https://arxiv.org/abs/1807.01989v3)]
- <a name="PSDDN"></a> **[PSDDN]** Point in, Box out: Beyond Counting Persons in Crowds (**CVPR(oral)**)[[paper](https://arxiv.org/abs/1904.01333)]
- <a name="ADCrowdNet"></a> **[ADCrowdNet]** ADCrowdNet: An Attention-injective Deformable Convolutional Network for Crowd Understanding (**CVPR**) [[paper](https://arxiv.org/abs/1811.11968)]
- <a name="CCWld"></a> **[CCWld, SFCN]** Learning from Synthetic Data for Crowd Counting in the Wild (**CVPR**) [[paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_Learning_From_Synthetic_Data_for_Crowd_Counting_in_the_Wild_CVPR_2019_paper.pdf)] [[Project](https://gjy3035.github.io/GCC-CL/)] [[arxiv](https://arxiv.org/abs/1903.03303)] ![GitHub stars](https://img.shields.io/github/stars/gjy3035/GCC-CL.svg?logo=github&label=Stars)
- <a name="DG-GAN"></a> **[DG-GAN]** Dense Crowd Counting Convolutional Neural Networks with Minimal Data using Semi-Supervised Dual-Goal Generative Adversarial Networks (**CVPRW**)[[paper](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Weakly%20Supervised%20Learning%20for%20Real-World%20Computer%20Vision%20Applications/Olmschenk_Dense_Crowd_Counting_Convolutional_Neural_Networks_with_Minimal_Data_using_CVPRW_2019_paper.pdf)]
- <a name="GSP"></a> **[GSP]** Global Sum Pooling: A Generalization Trick for Object Counting with Small Datasets of Large Images (**CVPRW**)[[paper](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Deep%20Vision%20Workshop/Aich_Global_Sum_Pooling_A_Generalization_Trick_for_Object_Counting_with_CVPRW_2019_paper.pdf)]
- <a name="IA-DNN"></a> **[IA-DNN]** Inverse Attention Guided Deep Crowd Counting Network (**AVSS Best Paper**) [[paper](https://arxiv.org/abs/1907.01193)]
- <a name="MTCNet"></a> **[MTCNet]** MTCNET: Multi-task Learning Paradigm for Crowd Count Estimation (**AVSS**) [[paper](https://arxiv.org/abs/1908.08652)]
- <a name="CODA"></a> **[CODA]** CODA: Counting Objects via Scale-aware Adversarial Density Adaption (**ICME**) [[paper](https://arxiv.org/abs/1903.10442)][[code](https://github.com/Willy0919/CODA)]![GitHub stars](https://img.shields.io/github/stars/Willy0919/CODA.svg?logo=github&label=Stars)
- <a name="LSTN"></a> **[LSTN]** Locality-Constrained Spatial Transformer Network for Video Crowd Counting (**ICME(oral)**)  [[paper](https://arxiv.org/abs/1907.07911)]
- <a name="DRD"></a> **[DRD]** Dynamic Region Division for Adaptive Learning Pedestrian Counting (**ICME**) [[paper](https://arxiv.org/abs/1908.03978)]
- <a name="MVSAN"></a> **[MVSAN]** Crowd Counting via Multi-View Scale Aggregation Networks (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8784912)]
- <a name="ASD"></a> **[ASD]** Adaptive Scenario Discovery for Crowd Counting (**ICASSP**) [[paper](https://arxiv.org/abs/1812.02393)]
- <a name="SAAN"></a> **[SAAN]** Crowd Counting Using Scale-Aware Attention Networks (**WACV**) [[paper](http://www.cs.umanitoba.ca/~ywang/papers/wacv19.pdf)]
- <a name="SPN"></a> **[SPN]** Scale Pyramid Network for Crowd Counting (**WACV**) [[paper](http://ieeexplore.ieee.org/xpl/mostRecentIssue.jsp?punumber=8642793)]
- <a name="GWTA-CCNN"></a> **[GWTA-CCNN]** Almost Unsupervised Learning for Dense Crowd Counting (**AAAI**) [[paper](http://val.serc.iisc.ernet.in/valweb/papers/AAAI_2019_WTACNN.pdf)]
- <a name="GPC"></a> **[GPC]** Geometric and Physical Constraints for Drone-Based Head Plane Crowd Density Estimation (**IROS**) [[paper](https://arxiv.org/abs/1803.08805)]
- <a name="AM-CNN"></a> **[AM-CNN]** Attention to Head Locations for Crowd Counting (**ICIG**) [[paper](https://arxiv.org/abs/1806.10287)]
- <a name="CRDNet"></a> **[CRDNet]** Cascaded Residual Density Network for Crowd Counting (**ICIP**) [[paper](https://arxiv.org/abs/2107.13718)]

### Journal
- <a name="D-ConvNet"></a> **[D-ConvNet]** Nonlinear Regression via Deep Negative Correlation Learning (**T-PAMI**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8850209)](extension of [D-ConvNet](#D-ConvNet))[[Project](https://mmcheng.net/dncl/)]
- <a name="SL2R"></a>  **[SL2R]** Exploiting Unlabeled Data in CNNs by Self-supervised Learning to Rank (**T-PAMI**) [[paper](https://arxiv.org/abs/1902.06285)](extension of [L2R](#L2R))
- <a name="PCC-Net"></a> **[PCC-Net]** PCC Net: Perspective Crowd Counting via Spatial Convolutional Network (**T-CSVT**) [[paper](https://arxiv.org/abs/1905.10085)] [[code](https://github.com/gjy3035/PCC-Net)]![GitHub stars](https://img.shields.io/github/stars/gjy3035/PCC-Net.svg?logo=github&label=Stars)
- <a name="Deem"></a> **[Deem]** Scale-Aware Crowd Counting via Depth-Embedded Convolutional Neural Networks (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8846233)]
- <a name="CLPC"></a> **[CLPC]** Cross-Line Pedestrian Counting Based on Spatially-Consistent Two-Stage Local Crowd Density Estimation and Accumulation (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8295124)]
- <a name="MAN"></a> **[MAN]** Mask-aware networks for crowd counting (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8796427)]
- <a name=""></a>Generalizing semi-supervised generative adversarial networks to regression using feature contrasting (**CVIU**)[[paper](https://arxiv.org/abs/1811.11269)]
- <a name="CCLL"></a> **[CCLL]** Crowd Counting With Limited Labeling Through Submodular Frame Selection (**T-ITS**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8360780)]
- <a name="MLCNN"></a> **[GMLCNN]** Learning Multi-Level Density Maps for Crowd Counting (**T-NNLS**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8848475)]
- <a name="HA-CCN"></a> **[HA-CCN]** HA-CCN: Hierarchical Attention-based Crowd Counting Network (**TIP**) [[paper](https://arxiv.org/abs/1907.10255)]
- <a name="PaDNet"></a> **[PaDNet]** PaDNet: Pan-Density Crowd Counting (**TIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8897143)]
- <a name="LDL"></a> **[LDL]** Indoor Crowd Counting by Mixture of Gaussians Label Distribution Learning (**TIP**) [[paper](http://palm.seu.edu.cn/xgeng/files/tip19.pdf)]
- <a name="ACSPNet"></a> **[ACSPNet]** Atrous convolutions spatial pyramid network for crowd counting and density estimation (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231219304059)]
- <a name="DDCN"></a> **[DDCN]** Removing background interference for crowd counting via de-background detail convolutional network (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231218315042)]
- <a name="MRA-CNN"></a> **[MRA-CNN]** Multi-resolution attention convolutional neural network for crowd counting (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231218312542)]
- <a name="ACM-CNN"></a> **[ACM-CNN]** Attend To Count: Crowd Counting with Adaptive Capacity Multi-scale CNNs (**Neurocomputing**) [[paper](https://arxiv.org/abs/1908.02797)]
- <a name="SDA-MCNN"></a> **[SDA-MCNN]** Counting crowds using a scale-distribution-aware network and adaptive human-shaped kernel (**Neurocomputing**) [[paper](https://www.sciencedirect.com/science/article/pii/S0925231219314651)]
- <a name="SCAR"></a> **[SCAR]** SCAR: Spatial-/Channel-wise Attention Regression Networks for Crowd Counting (**Neurocomputing**) [[paper](https://arxiv.org/abs/1908.03716)][[code](https://github.com/gjy3035/SCAR)]![GitHub stars](https://img.shields.io/github/stars/gjy3035/SCAR.svg?logo=github&label=Stars)

### 2018
### Conference
- <a name="SANet"></a> **[SANet]** Scale Aggregation Network for Accurate and Efficient Crowd Counting (**ECCV**) [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xinkun_Cao_Scale_Aggregation_Network_ECCV_2018_paper.pdf)]
- <a name="ic-CNN"></a> **[ic-CNN]** Iterative Crowd Counting (**ECCV**) [[paper](https://arxiv.org/abs/1807.09959)]
- <a name="CL"></a> **[CL]** Composition Loss for Counting, Density Map Estimation and Localization in Dense Crowds (**ECCV**) [[paper](https://arxiv.org/abs/1808.01050)]
- <a name="LCFCN"></a> **[LCFCN]**  Where are the Blobs: Counting by Localization with Point Supervision (**ECCV**) [[paper](https://arxiv.org/abs/1807.09856)] [[code](https://github.com/ElementAI/LCFCN)]![GitHub stars](https://img.shields.io/github/stars/ElementAI/LCFCN.svg?logo=github&label=Stars)
- <a name="CSR"></a> **[CSR]**  CSRNet: Dilated Convolutional Neural Networks for Understanding the Highly Congested Scenes (**CVPR**) [[paper](https://arxiv.org/abs/1802.10062)] [[code](https://github.com/leeyeehoo/CSRNet-pytorch)]![GitHub stars](https://img.shields.io/github/stars/leeyeehoo/CSRNet-pytorch.svg?logo=github&label=Stars)
- <a name="L2R"></a>  **[L2R]** Leveraging Unlabeled Data for Crowd Counting by Learning to Rank (**CVPR**) [[paper](https://arxiv.org/abs/1803.03095)] [[code](https://github.com/xialeiliu/CrowdCountingCVPR18)] ![GitHub stars](https://img.shields.io/github/stars/xialeiliu/CrowdCountingCVPR18.svg?logo=github&label=Stars)
- <a name="ACSCP"></a> **[ACSCP]**  Crowd Counting via Adversarial Cross-Scale Consistency Pursuit  (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Shen_Crowd_Counting_via_CVPR_2018_paper.pdf)]   [unofficial code: [PyTorch](https://github.com/RQuispeC/pytorch-ACSCP)]![GitHub stars](https://img.shields.io/github/stars/RQuispeC/pytorch-ACSCP.svg?logo=github&label=Stars)
- <a name="DecideNet"></a> **[DecideNet]** DecideNet: Counting Varying Density Crowds Through Attention Guided Detection and Density (**CVPR**) [[paper](https://arxiv.org/abs/1712.06679)]
- <a name="AMDCN"></a>  **[AMDCN]** An Aggregated Multicolumn Dilated Convolution Network for Perspective-Free Counting (**CVPRW**) [[paper](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w6/Deb_An_Aggregated_Multicolumn_CVPR_2018_paper.pdf)] [[code](https://github.com/diptodip/counting)] ![GitHub stars](https://img.shields.io/github/stars/diptodip/counting.svg?logo=github&label=Stars)
- <a name="D-ConvNet"></a> **[D-ConvNet]** Crowd Counting with Deep Negative Correlation Learning (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Shi_Crowd_Counting_With_CVPR_2018_paper.pdf)] [[code](https://github.com/shizenglin/Deep-NCL)]![GitHub stars](https://img.shields.io/github/stars/shizenglin/Deep-NCL.svg?logo=github&label=Stars)
- <a name="IG-CNN"></a> **[IG-CNN]** Divide and Grow: Capturing Huge Diversity in Crowd Images with
Incrementally Growing CNN (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Sam_Divide_and_Grow_CVPR_2018_paper.pdf)]
- <a name="SCNet"></a>**[SCNet]** In Defense of Single-column Networks for Crowd Counting (**BMVC**) [[paper](https://arxiv.org/abs/1808.06133)]
- <a name="AFP"></a>**[AFP]** Crowd Counting by Adaptively Fusing Predictions from an Image Pyramid (**BMVC**) [[paper](https://arxiv.org/abs/1805.06115)]
- <a name="DRSAN"></a>**[DRSAN]** Crowd Counting using Deep Recurrent Spatial-Aware Network (**IJCAI**) [[paper](https://arxiv.org/abs/1807.00601)]
- <a name="TDF-CNN"></a>**[TDF-CNN]** Top-Down Feedback for Crowd Counting Convolutional Neural Network (**AAAI**) [[paper](https://arxiv.org/abs/1807.08881)]
- <a name="CAC"></a>**[CAC]** Class-Agnostic Counting (**ACCV**) [[paper](https://arxiv.org/abs/1811.00472)] [[code](https://github.com/erikalu/class-agnostic-counting)]![GitHub stars](https://img.shields.io/github/stars/erikalu/class-agnostic-counting.svg?logo=github&label=Stars)
- <a name="A-CCNN"></a> **[A-CCNN]** A-CCNN: Adaptive CCNN for Density Estimation and Crowd Counting (**ICIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8451399)]
- <a name=""></a> Crowd Counting with Fully Convolutional Neural Network (**ICIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8451787)]
- <a name="MS-GAN"></a> **[MS-GAN]** Multi-scale Generative Adversarial Networks for Crowd Counting (**ICPR**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8545683)]
- <a name="DR-ResNet"></a> **[DR-ResNet]** A Deeply-Recursive Convolutional Network for Crowd Counting (**ICASSP**) [[paper](https://arxiv.org/abs/1805.05633)] 
- <a name="GAN-MTR"></a> **[GAN-MTR]** Crowd Counting With Minimal Data Using Generative Adversarial Networks For Multiple Target Regression (**WACV**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8354235)]
- <a name="SaCNN"></a> **[SaCNN]** Crowd counting via scale-adaptive convolutional neural network (**WACV**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8354231)] [[code](https://github.com/miao0913/SaCNN-CrowdCounting-Tencent_Youtu)]![GitHub stars](https://img.shields.io/github/stars/miao0913/SaCNN-CrowdCounting-Tencent_Youtu.svg?logo=github&label=Stars)

### Journal
- <a name="BSAD"></a> **[BSAD]** Body Structure Aware Deep Crowd Counting (**TIP**) [[paper](http://mac.xmu.edu.cn/rrji/papers/IP%202018-Body.pdf)] 
- <a name="NetVLAD"></a> **[NetVLAD]** Multiscale Multitask Deep NetVLAD for Crowd Counting (**TII**) [[paper](https://staff.fnwi.uva.nl/z.shi/files/counting-netvlad.pdf)] [[code](https://github.com/shizenglin/Multitask-Multiscale-Deep-NetVLAD)]![GitHub stars](https://img.shields.io/github/stars/shizenglin/Multitask-Multiscale-Deep-NetVLAD.svg?logo=github&label=Stars)
- <a name="W-VLAD"></a> **[W-VLAD]** Crowd Counting via Weighted VLAD on Dense Attribute Feature Maps (**T-CSVT**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7778134)]
- <a name="Improved SaCNN"></a> **[Improved SaCNN]** Improved Crowd Counting Method Based on Scale-Adaptive Convolutional Neural Network (**IEEE Access**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8643345)]
- <a name="DA-Net"></a> **[DA-Net]** DA-Net: Learning the Fine-Grained Density Distribution With Deformation Aggregation Network (**IEEE Access**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8497050)][[code](https://github.com/BigTeacher-777/DA-Net)]![GitHub stars](https://img.shields.io/github/stars/BigTeacher-777/DA-Net.svg?logo=github&label=Stars)

### 2017
### Conference
- <a name="SCNN"></a> **[Switching CNN]** Switching Convolutional Neural Network for Crowd Counting (**CVPR**) [[paper](https://arxiv.org/abs/1708.00199)] [[code](https://github.com/val-iisc/crowd-counting-scnn)]![GitHub stars](https://img.shields.io/github/stars/val-iisc/crowd-counting-scnn.svg?logo=github&label=Stars)
- <a name="CP-CNN"></a> **[CP-CNN]** Generating High-Quality Crowd Density Maps using Contextual Pyramid CNNs (**ICCV**) [[paper](https://arxiv.org/abs/1708.00953)]
- <a name="ConvLSTM"></a> **[ConvLSTM]** Spatiotemporal Modeling for Crowd Counting in Videos (**ICCV**) [[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Xiong_Spatiotemporal_Modeling_for_ICCV_2017_paper.pdf)]
- <a name="CMTL"></a> **[CMTL]** CNN-based Cascaded Multi-task Learning of High-level Prior and Density Estimation for Crowd Counting (**AVSS**) [[paper](https://arxiv.org/abs/1707.09605)] [[code](https://github.com/svishwa/crowdcount-cascaded-mtl)]![GitHub stars](https://img.shields.io/github/stars/svishwa/crowdcount-cascaded-mtl.svg?logo=github&label=Stars)
- <a name="ResnetCrowd"></a> **[ResnetCrowd]** ResnetCrowd: A Residual Deep Learning Architecture for Crowd Counting, Violent Behaviour Detection and Crowd Density Level Classification (**AVSS**) [[paper](https://arxiv.org/abs/1705.10698)]
- <a name="ACNN"></a> **[ACNN]** Incorporating Side Information by Adaptive Convolution (**NeurIPS**) [[paper](http://papers.nips.cc/paper/6976-incorporating-side-information-by-adaptive-convolution.pdf)][[Project](http://visal.cs.cityu.edu.hk/research/acnn/)]
- <a name="MSCNN"></a> **[MSCNN]** Multi-scale Convolution Neural Networks for Crowd Counting (**ICIP**) [[paper](https://arxiv.org/abs/1702.02359)] [[code](https://github.com/Ling-Bao/mscnn)]![GitHub stars](https://img.shields.io/github/stars/Ling-Bao/mscnn.svg?logo=github&label=Stars)
- <a name="FCNCC"></a> **[FCNCC]** Fully Convolutional Crowd Counting On Highly Congested Scenes (**VISAPP**) [[paper](https://arxiv.org/abs/1612.00220)]

### Journal
- <a name="DAL-SVR"></a> **[DAL-SVR]** Boosting deep attribute learning via support vector regression for fast moving crowd counting (**PR Letters**) [[paper](https://www.sciencedirect.com/science/article/pii/S0167865517304415)]
- <a name="CNN-MRF"></a> **[CNN-MRF]** Image Crowd Counting Using Convolutional Neural Network and Markov Random Field (**JACII**) [[paper](https://arxiv.org/abs/1706.03686)] [[code](https://github.com/hankong/crowd-counting)]![GitHub stars](https://img.shields.io/github/stars/hankong/crowd-counting.svg?logo=github&label=Stars)


### 2016 
### Conference
- <a name="MCNN"></a> **[MCNN]** Single-Image Crowd Counting via Multi-Column Convolutional Neural Network (**CVPR**) [[paper](https://pdfs.semanticscholar.org/7ca4/bcfb186958bafb1bb9512c40a9c54721c9fc.pdf)] [unofficial code: [TensorFlow](https://github.com/aditya-vora/crowd_counting_tensorflow) ![GitHub stars](https://img.shields.io/github/stars/aditya-vora/crowd_counting_tensorflow.svg?logo=github&label=Stars) [PyTorch](https://github.com/svishwa/crowdcount-mcnn)]![GitHub stars](https://img.shields.io/github/stars/svishwa/crowdcount-mcnn.svg?logo=github&label=Stars)
- <a name="Hydra-CNN"></a> **[Hydra-CNN]** Towards perspective-free object counting with deep learning  (**ECCV**) [[paper](http://agamenon.tsc.uah.es/Investigacion/gram/publications/eccv2016-onoro.pdf)] [[code](https://github.com/gramuah/ccnn)]![GitHub stars](https://img.shields.io/github/stars/gramuah/ccnn.svg?logo=github&label=Stars)
- <a name="CNN-Boosting"></a> **[CNN-Boosting]** Learning to Count with CNN Boosting (**ECCV**) [[paper](https://link.springer.com/chapter/10.1007%2F978-3-319-46475-6_41)] 
- <a name="Crossing-line"></a> **[Crossing-line]** Crossing-line Crowd Counting with Two-phase Deep Neural Networks (**ECCV**) [[paper](https://www.ee.cuhk.edu.hk/~xgwang/papers/ZhaoLZWeccv16.pdf)] 
- <a name="GP"></a> **[GP]** Gaussian Process Density Counting from Weak Supervision (**ECCV**) [[paper](https://link.springer.com/chapter/10.1007%2F978-3-319-46448-0_22)]
- <a name="CrowdNet"></a> **[CrowdNet]** CrowdNet: A Deep Convolutional Network for Dense Crowd Counting (**ACMMM**) [[paper](https://arxiv.org/abs/1608.06197)] [[code](https://github.com/davideverona/deep-crowd-counting_crowdnet)]![GitHub stars](https://img.shields.io/github/stars/davideverona/deep-crowd-counting_crowdnet.svg?logo=github&label=Stars)
- <a name="Shang2016"></a> **[Shang 2016]** End-to-end crowd counting via joint learning local and global count (**ICIP**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7532551)]
- <a name="DE-VOC"></a> **[DE-VOC]** Fast visual object counting via example-based density estimation (**ICIP**) [[paper](http://web.pkusz.edu.cn/adsp/files/2015/10/Fast-Visual-Object-Counting-via-Example-based-Density-Estimation.pdf)] 
- <a name="RPF"></a> **[RPF]** Crowd Density Estimation based on Rich Features and Random Projection Forest (**WACV**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7477682)] 
- <a name="CS-SLR"></a> **[CS-SLR]** Cost-sensitive sparse linear regression for crowd counting with imbalanced training data (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7552905)] 
- <a name="Faster-OHEM-KCF"></a> **[Faster-OHEM-KCF]** Deep People Counting with Faster R-CNN and Correlation Tracking (**ICME**) [[paper](https://dl.acm.org/citation.cfm?id=3007745)] 

### 2015
### Conference
- <a name="COUNTForest"></a> **[COUNT Forest]** COUNT Forest: CO-voting Uncertain Number of Targets using Random Forest
for Crowd Density Estimation (**ICCV**) [[paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Pham_COUNT_Forest_CO-Voting_ICCV_2015_paper.pdf)]
- <a name="Bayesian"></a> **[Bayesian]** Bayesian Model Adaptation for Crowd Counts (**ICCV**) [[paper](https://ieeexplore.ieee.org/document/7410832?arnumber=7410832&tag=1)]
- <a name="Zhang2015"></a> **[Zhang 2015]** Cross-scene Crowd Counting via Deep Convolutional Neural Networks (**CVPR**) [[paper](https://www.ee.cuhk.edu.hk/~xgwang/papers/zhangLWYcvpr15.pdf)] [[code](https://github.com/wk910930/crowd_density_segmentation)]![GitHub stars](https://img.shields.io/github/stars/wk910930/crowd_density_segmentation.svg?logo=github&label=Stars)
- <a name="Wang2015"></a> **[Wang 2015]** Deep People Counting in Extremely Dense Crowds (**ACMMM**) [[paper](https://dl.acm.org/citation.cfm?id=2806337)]

### Journal
- <a name="Fu2015"></a> **[FU 2015]** Fast crowd density estimation with convolutional neural networks (**Artificial Intelligence**) [[paper](https://www.sciencedirect.com/science/article/pii/S0952197615000871)]

### 2014
### Conference
- <a name="Arteta2014"></a> **[Arteta 2014]** Interactive Object Counting (**ECCV**) [[paper](http://vigir.missouri.edu/~gdesouza/Research/Conference_CDs/ECCV_2014/papers/8691/86910504.pdf)] 

### 2013
### Conference
- <a name="Idrees2013"></a> **[Idrees 2013]** Multi-Source Multi-Scale Counting in Extremely Dense Crowd Images (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2013/papers/Idrees_Multi-source_Multi-scale_Counting_2013_CVPR_paper.pdf)]
- <a name="Ma2013"></a> **[Ma 2013]** Crossing the Line: Crowd Counting by Integer Programming with Local Features (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2013/papers/Ma_Crossing_the_Line_2013_CVPR_paper.pdf)]
- <a name="Chen2013"></a> **[Chen 2013]** Cumulative Attribute Space for Age and Crowd Density Estimation (**CVPR**) [[paper](http://openaccess.thecvf.com/content_cvpr_2013/papers/Chen_Cumulative_Attribute_Space_2013_CVPR_paper.pdf)]
- <a name="SSR"></a> **[SSR]** From Semi-Supervised to Transfer Counting of Crowds (**ICCV**) [[paper](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Loy_From_Semi-supervised_to_2013_ICCV_paper.pdf)]

### 2012
### Conference
- <a name="Chen2012"></a> **[Chen 2012]** Feature mining for localised crowd counting (**BMVC**) [[paper](https://pdfs.semanticscholar.org/c5ec/65e36bccf8a64050d38598511f0352653d6f.pdf)]

### 2011
### Conference
- <a name="Rodriguez2011"></a> **[Rodriguez 2011]** Density-aware person detection and tracking in crowds (**ICCV**) [[paper](https://hal-enpc.archives-ouvertes.fr/hal-00654266/file/ICCV11a.pdf)]

### 2010
### Conference
- <a name="Lempitsky2010"></a> **[Lempitsky 2010]** Learning To Count Objects in Images (**NeurIPS**) [[paper](http://papers.nips.cc/paper/4043-learning-to-count-objects-in-images)]

### 2008
### Conference
- <a name="Chan2008"></a> **[Chan 2008]** Privacy preserving crowd monitoring: Counting people without people models or tracking (**CVPR**) [[paper](http://visal.cs.cityu.edu.hk/static/pubs/conf/cvpr08-peoplecnt.pdf)]



## Leaderboard
The section is being continually updated. Note that some values have superscript, which indicates their source. 

### NWPU

Please refer to [this page](https://www.crowdbenchmark.com/nwpucrowd.html).

### ShanghaiTech Part A

| Year-Conference/Journal | Methods           | MAE   | MSE   | PSNR  | SSIM | Params | Pre-trained   Model |
| ---- | ------------------------------------ | ----- | ----- | ----- | ---- | ------ | ------------------- |
| 2016--CVPR | [MCNN](#MCNN)     | 110.2 | 173.2 | 21.4<sup>[CSR](#CSR)</sup> | 0.52<sup>[CSR](#CSR)</sup>  | 0.13M<sup>[SANet](#SANet)</sup>  | None  |
| 2017--AVSS | [CMTL](#CMTL)                                | 101.3 | 152.4 | -  | -  | -  | None        |
| 2017--CVPR | [Switching CNN](#SCNN)                       | 90.4  | 135.0 | -  | -  | 15.11M<sup>[SANet](#SANet)</sup>  | VGG-16      |
| 2017--ICIP | [MSCNN](#MSCNN)                              | 83.8  | 127.4 | -  | -  | -  | -           |
| 2017--ICCV | [CP-CNN](#CP-CNN) | 73.6  | 106.4 | 21.72<sup>[CP-CNN](#CP-CNN)</sup> | 0.72<sup>[CP-CNN](#CP-CNN)</sup>  | 68.4M<sup>[SANet](#SANet)</sup>  | - |
| 2018--AAAI | [TDF-CNN](#TDF-CNN)                          | 97.5  | 145.1 | -  | -  | -  | -           |
| 2018--WACV | [SaCNN](#SaCNN)                              | 86.8  | 139.2 | -  | -  | -  | -           |
| 2018--CVPR | [ACSCP](#ACSCP)                              | 75.7  | 102.7 | -  | -  | 5.1M | None      |
| 2018--CVPR | [D-ConvNet-v1](#D-ConvNet)                   | 73.5  | 112.3 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [IG-CNN](#IG-CNN)                            | 72.5  | 118.2 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Query-by-example) | 72.0  | 106.6 | -  | -  | -  | VGG-16      |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Keyword)          | 73.6  | 112.0 | -  | -  | -  | VGG-16      |
| 2019--CVPRW| [GSP](#GSP) (one stage, efficient)           | 70.7  | 103.6 | -  | -  | -  | VGG-16      |
| 2018--IJCAI| [DRSAN](#DRSAN)                              | 69.3  | 96.4  | -  | -  | -  | -           |
| 2018--ECCV | [ic-CNN](#ic-CNN) (one stage)                | 69.8  | 117.3 | -  | -  | -  | -           |
| 2018--ECCV | [ic-CNN](#ic-CNN) (two stages)               | 68.5  | 116.2 | -  | -  | -  | -           |
| 2018--CVPR | [CSRNet](#CSR)   | 68.2  | 115.0 | 23.79 | 0.76 | 16.26M<sup>[SANet](#SANet)</sup> |VGG-16|
| 2018--ECCV | [SANet](#SANet)                              | 67.0  | 104.5 | -  | -  | 0.91M | None     |
| 2019--AAAI | [GWTA-CCNN](#GWTA-CCNN)                      | 154.7 | 229.4 | -  | -  | -  | -           |
| 2021--TPAMI| [LA-Batch](#LA-Batch) (backbone CSRNet)      | 65.8  | 103.6 | -  | -  | -  | -           |
| 2019--ICASSP | [ASD](#ASD)                                | 65.6  | 98.0  | -  | -  | -  | -           |
| 2019--ICCV | [CFF](#CFF)                                  | 65.2  | 109.4 | 25.4  | 0.78 | -     | -   |
| 2019--CVPR | [SFCN](#CCWld)                               | 64.8  | 107.5 | -  | -  | -  | -           |
| 2020--AAAI | [DUBNet](#DUBNet)                            | 64.6  | 106.8 | -  | -  | -  | -           |
| 2019--ICCV | [SPN+L2SM](#L2SM)                            | 64.2  | 98.4  | -  | -  | -  | -           |
| 2019--CVPR | [TEDnet](#TEDnet)                            | 64.2  | 109.1 | 25.88 | 0.83 | 1.63M | -   |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-bAttn-DME)     | 63.2  | 98.9  | 24.48 | 0.88 | -     | -   |
| 2019--CVPR | [PACNN](#PACNN)                              | 66.3  | 106.4 | -  | -  | -  | -           |
| 2019--CVPR | [PACNN+CSRNet](#PACNN)                       | 62.4  | 102.0 | -  | -  | -  | -           |
| 2019--CVPR | [CAN](#CAN)                                  | 62.3  | 100.0 | -  | -  | -  | VGG-16      |
| 2019--TIP  | [HA-CCN](#HA-CCN)                            | 62.9  | 94.9  | -  | -  | -  | -           |
| 2019--ICCV | [BL](#BL)                                    | 62.8  | 101.8 | -  | -  | -  | -           |
| 2019--WACV | [SPN](#SPN)                                  | 61.7  | 99.5  | -  | -  | -  | -           |
| 2019--ICCV | [DSSINet](#DSSINet)                          | 60.63 | 96.04 | -  | -  | -  | -           |
| 2019--ICCV | [MBTTBF-SCFB](#MBTTBF)                       | 60.2  | 94.1  | -  | -  | -  | -           |
| 2019--ICCV | [RANet](#RANet)                              | 59.4  | 102.0 | -  | -  | -  | -           |
| 2019--ICCV | [SPANet+SANet](#SPANet)                      | 59.4  | 92.5  | -  | -  | -  | -           |
| 2019--TIP  | [PaDNet](#PaDNet)                            | 59.2  | 98.1  | -  | -  | -  | -           |
| 2022--CVPR | [GauNet](#GauNet)                           | 59.2  | 95.4  | -  | -  | -  | VGG-16      |
| 2019--ICCV | [S-DCNet](#S-DCNet)                          | 58.3  | 95.0  | -  | -  | -  | -           |
| 2020--ICPR | [M-SFANet+M-SegNet](#M-SFANet)               | 57.55 | 94.48 | -  | -  | -  | -           |
| 2019--ICCV |**[PGCNet](#PGCNet)**                         | 57.0 | **86.0** | -  | -  | -  | -         |
| 2020--ECCV | [AMSNet](#AMSNet)                            | 56.7 | 93.4   | -  | -  | -  | -             |
| 2020--CVPR | [ADSCNet](#ADSCNet)                          | 55.4 | 97.7   | -  | -  | -  | -           |
| 2021--AAAI |**[SASNet](#SASNet)**                         | **53.59** | 88.38 | -  | -  | -  | -       |



### ShanghaiTech Part B

| Year-Conference/Journal | Methods                          | MAE   | MSE   |
| ---- | ---------------- | ----- | ---- |
| 2016--CVPR | [MCNN](#MCNN)                                 | 26.4  | 41.3  |
| 2017--ICIP | [MSCNN](#MSCNN)                               | 17.7  | 30.2  |
| 2017--AVSS | [CMTL](#CMTL)                                 | 20.0  | 31.1  |
| 2017--CVPR | [Switching CNN](#SCNN)                        | 21.6  | 33.4  |
| 2017--ICCV | [CP-CNN](#CP-CNN)                             | 20.1  | 30.1  |
| 2018--TIP  | [BSAD](#BSAD)                                 | 20.2  | 35.6  |
| 2018--WACV | [SaCNN](#SaCNN)                               | 16.2  | 25.8  |
| 2018--CVPR | [ACSCP](#ACSCP)                               | 17.2  | 27.4  |
| 2018--CVPR | [CSRNet](#CSR)                                | 10.6  | 16.0  |
| 2018--CVPR | [IG-CNN](#IG-CNN)                             | 13.6  | 21.1  |
| 2018--CVPR | [D-ConvNet-v1](#D-ConvNet)                    | 18.7  | 26.0  |
| 2018--CVPR | [DecideNet](#DecideNet)                       | 21.53 | 31.98 |
| 2018--CVPR | [DecideNet + R3](#DecideNet)                  | 20.75 | 29.42 |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Query-by-example)  | 14.4  | 23.8  |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Keyword)           | 13.7  | 21.4  |
| 2018--IJCAI| [DRSAN](#DRSAN)                               | 11.1  | 18.2  |
| 2018--AAAI | [TDF-CNN](#TDF-CNN)                           | 20.7  | 32.8  |
| 2018--ECCV | [ic-CNN](#ic-CNN) (one stage)                 | 10.4  | 16.7  |
| 2018--ECCV | [ic-CNN](#ic-CNN) (two stages)                | 10.7  | 16.0  |
| 2019--CVPRW| [GSP](#GSP) (one stage, efficient)            | 9.1   | 15.9  |
| 2021--TPAMI| [LA-Batch](#LA-Batch) (backbone CSRNet)       | 8.6   | 13.6  |
| 2018--ECCV | [SANet](#SANet)                               | 8.4   | 13.6  |
| 2019--WACV | [SPN](#SPN)                                   | 9.4   | 14.4  |
| 2019--ICCV | [PGCNet](#PGCNet)                             | 8.8   | 13.7  |
| 2019--ICASSP | [ASD](#ASD)                                 | 8.5   | 13.7  |
| 2019--CVPR | [TEDnet](#TEDnet)                             | 8.2   | 12.8  |
| 2019--TIP  | [HA-CCN](#HA-CCN)                             | 8.1   | 13.4  |
| 2019--TIP  | [PaDNet](#PaDNet)                             | 8.1   | 12.2  |
| 2019--ICCV | [RANet](#RANet)                               | 7.9   | 12.9  |
| 2019--CVPR | [CAN](#CAN)                                   | 7.8   | 12.2  |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-attn-DME)       | 7.7   | 12.9  |
| 2020--AAAI | [DUBNet](#DUBNet)                             | 7.7   | 12.5  |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-DME)            | 7.6   | 13.9  |
| 2019--CVPR | [SFCN](#CCWld)                                | 7.6   | 13.0  |
| 2019--CVPR | [PACNN](#PACNN)                               | 8.9   | 13.5  |
| 2022--CVPR | [GauNet](#GauNet)(VGG-16)                     | 7.6   | 12.7  |
| 2019--CVPR | [PACNN+CSRNet](#PACNN)                        | 7.6   | 11.8  |
| 2019--ICCV | [BL](#BL)                                     | 7.7   | 12.7  |
| 2019--ICCV | [CFF](#CFF)                                   | 7.2   | 12.2  |
| 2019--ICCV | [SPN+L2SM](#L2SM)                             | 7.2   | 11.1  |
| 2019--ICCV | [DSSINet](#DSSINet)                           | 6.85  | 10.34 |
| 2019--ICCV | [S-DCNet](#S-DCNet)                           | 6.7   | 10.7  |
| 2019--ICCV | **[SPANet+SANet](#SPANet)**                   | 6.5   | **9.9** |
| 2020--CVPR | [ADSCNet](#ADSCNet)                           | 6.4   | 11.3 |
| 2020--ICPR | **[M-SFANet+M-SegNet](#M-SFANet)**            | **6.32** | 10.06 |
| 2021--AAAI | **[SASNet](#SASNet)**                         | 6.35  | **9.9** |

### JHU-CROWD++

| Year-Conference/Journal | Methods                          | MAE(Val Set)   | MSE(Val Set)   | MAE(Test Set)   | MSE(Test Set)   |
| ---- | ---------------- | ----- | ---- | ----- | ---- |
| 2016--CVPR | [MCNN](#MCNN)                                 | 160.6 | 377.7  | 188.9 | 483.4  |
| 2017--AVSS | [CMTL](#CMTL)                                 | 138.1 | 379.5  | 157.8 | 490.4  |
| 2019--ICCV | [DSSINet](#DSSINet)                           | 116.6 | 317.4  | 133.5 | 416.5  |
| 2019--CVPR | [CAN](#CAN)                                   | 89.5  | 239.3  | 100.1 | 314.0  |
| 2020--TPAMI | [LSC-CNN](#LSC-CNN)                          | 87.3  | 309.0  | 112.7 | 454.4  |  
| 2018--ECCV | [SANet](#SANet)                               | 82.1  | 272.6  | 91.1  | 320.4  |
| 2019--ICCV | [MBTTBF](#MBTTBF)                             | 73.8  | 256.8  | 81.8  | 299.1  |  
| 2018--CVPR | [CSRNet](#CSR)                                | 72.2  | 249.9  | 85.9  | 309.2  |
| 2022--CVPR | [GauNet](#GauNet)(VGG-16)                     | -     | -      | 69.4  | 262.4  |
| 2020--TPAMI | [CG-DRCN-CC-VGG16](#JHU-CROWD)               | 67.9  | 262.1  | 82.3  | 328.0  |
| 2019--CVPR | [SFCN](#CCWld)                                | 62.9  | 247.5  | 77.5  | 297.6  |  
| 2019--ICCV | **[BL](#BL)**                                 | 59.3  | **229.2**  | 75.0  | 299.9  |
| 2020--TPAMI | **[CG-DRCN-CC-Res101](#JHU-CROWD)**          | **57.6**  | 244.4  | **71.0** | **278.6**  |



### UCF-QNRF

| Year-Conference/Journal | Method | C-MAE | C-NAE | C-MSE | DM-MAE | DM-MSE | DM-HI | L- Av. Precision	| L-Av. Recall | L-AUC |
| --- | --- | --- | --- |--- | --- | --- |--- | --- | --- | ---|
| 2013--CVPR | [Idrees 2013](#Idrees2013)<sup>[CL](#CL)</sup>| 315 | 0.63 | 508 | - | - | - | - | - | - |
| 2016--CVPR | [MCNN](#MCNN)<sup>[CL](#CL)</sup> | 277 | 0.55 | 426 |0.006670| 0.0223 | 0.5354 |59.93% | 63.50% | 0.591|
| 2017--AVSS | [CMTL](#CMTL)<sup>[CL](#CL)</sup>            | 252 | 0.54 | 514 | 0.005932 | 0.0244 | 0.5024 | - | - | - |
| 2017--CVPR | [Switching CNN](#SCNN)<sup>[CL](#CL)</sup>   | 228 | 0.44 | 445 | 0.005673 | 0.0263 | 0.5301 | - | - | - |
| 2018--ECCV | [CL](#CL)     | 132 | 0.26 | 191 | 0.00044| 0.0017 | 0.9131 | 75.8% | 59.75%	| 0.714|
| 2019--TIP  | [HA-CCN](#HA-CCN)   | 118.1 | - | 180.4 | - | - | - | - | - | - |
| 2019--CVPR | [TEDnet](#TEDnet)   | 113   | - | 188   | - | - | - | - | - | - |
| 2021--TPAMI| [LA-Batch](#LA-Batch)| 113  | - | 210   | - | - | - | - | - | - |
| 2019--ICCV | [RANet](#RANet)     | 111   | - | 190   | - | - | - | - | - | - |
| 2019--CVPR | [CAN](#CAN)         | 107   | - | 183   | - | - | - | - | - | - |
| 2020--AAAI | [DUBNet](#DUBNet)   | 105.6 | - | 180.5 | - | - | - | - | - | - |
| 2019--ICCV | [SPN+L2SM](#L2SM)   | 104.7 | - | 173.6 | - | - | - | - | - | - |
| 2019--ICCV | [S-DCNet](#S-DCNet) | 104.4 | - | 176.1 | - | - | - | - | - | - |
| 2019--CVPR | [SFCN](#CCWld)      | 102.0 | - | 171.4 | - | - | - | - | - | - |
| 2019--ICCV | [DSSINet](#DSSINet) | 99.1  | - | 159.2 | - | - | - | - | - | - |
| 2019--ICCV | [MBTTBF-SCFB](#MBTTBF)      | 97.5 | - | 165.2 | - | - | - | - | - | - |
| 2019--TIP  | [PaDNet](#PaDNet)           | 96.5 | - | 170.2 | - | - | - | - | - | - |
| 2019--ICCV | [BL](#BL)                   | 88.7 | - | 154.8 | - | - | - | - | - | - |
| 2020--ICPR | [M-SFANet](#M-SFANet)       | 85.6 | - | 151.23 | - | - | - | - | - | - |
| 2021--AAAI | [SASNet](#SASNet)           | 85.2 | - | 147.3 | - | - | - | - | - | - |
| 2022--CVPR | [GauNet](#GauNet)(VGG-16)   | 84.2 | - | 152.4 | - | - | - | - | - | - |
| 2020--CVPR | **[ADSCNet](#ADSCNet)**     | **71.3** | - | **132.5** | - | - | - | - | - | - |


### UCF_CC_50

| Year-Conference/Journal | Methods                         | MAE   | MSE   |
| ---- | ---------------- | ----- | ---- |
| 2013--CVPR | [Idrees 2013](#Idrees2013)                   | 468.0 | 590.3  |
| 2015--CVPR | [Zhang 2015](#Zhang2015)                     | 467.0 | 498.5  |
| 2016--ACM MM | [CrowdNet](#CrowdNet)                      | 452.5 |   -    |
| 2016--CVPR | [MCNN](#MCNN)                                | 377.6 | 509.1  |
| 2016--ECCV | [CNN-Boosting](#CNN-Boosting)                | 364.4 |   -    |
| 2016--ECCV | [Hydra-CNN](#Hydra-CNN)                      | 333.73| 425.26 |
| 2016--ICIP | [Shang 2016](#Shang2016)                     | 270.3 |   -    |
| 2017--ICIP | [MSCNN](#MSCNN)                              | 363.7 | 468.4  |
| 2017--AVSS | [CMTL](#CMTL)                                | 322.8 | 397.9  |
| 2017--CVPR | [Switching CNN](#SCNN)                       | 318.1 | 439.2  |
| 2017--ICCV | [CP-CNN](#CP-CNN)                            | 298.8 | 320.9  |
| 2017--ICCV | [ConvLSTM-nt](#ConvLSTM)                     | 284.5 | 297.1  |
| 2018--TIP  | [BSAD](#BSAD)                                | 409.5 | 563.7  |
| 2018--AAAI | [TDF-CNN](#TDF-CNN)                          | 354.7 | 491.4  |
| 2018--WACV | [SaCNN](#SaCNN)                              | 314.9 | 424.8  |
| 2018--CVPR | [IG-CNN](#IG-CNN)                            | 291.4 | 349.4  |
| 2018--CVPR | [ACSCP](#ACSCP)                              | 291.0 | 404.6  |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Query-by-example) | 291.5 | 397.6  |
| 2018--CVPR | [L2R](#L2R) (Multi-task,   Keyword)          | 279.6 | 388.9  |
| 2018--CVPR | [D-ConvNet-v1](#D-ConvNet)                   | 288.4 | 404.7  |
| 2018--CVPR | [CSRNet](#CSR)                               | 266.1 | 397.5  |
| 2018--ECCV | [ic-CNN](#ic-CNN) (two stages)               | 260.9 | 365.5  |
| 2018--ECCV | [SANet](#SANet)                              | 258.4 | 334.9  |
| 2018--IJCAI| [DRSAN](#DRSAN)                              | 219.2 | 250.2  |
| 2019--AAAI | [GWTA-CCNN](#GWTA-CCNN)                      | 433.7 | 583.3  |
| 2019--WACV | [SPN](#SPN)                                  | 259.2 | 335.9  |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(DME)               | 257.1 | 363.5  |
| 2019--TIP  | [HA-CCN](#HA-CCN)                            | 256.2 | 348.4  |
| 2019--CVPR | [TEDnet](#TEDnet)                            | 249.4 | 354.5  |
| 2019--CVPR | [PACNN](#PACNN)                              | 267.9 | 357.8  |
| 2020--AAAI | [DUBNet](#DUBNet)                            | 243.8 | 329.3  |
| 2019--CVPR | [PACNN+CSRNet](#PACNN)                       | 241.7 | 320.7  |
| 2019--ICCV | [RANet](#RANet)                              | 239.8 | 319.4  |
| 2019--ICCV | [MBTTBF-SCFB](#MBTTBF)                       | 233.1 | 300.9  |
| 2019--ICCV | [BL](#BL)                                    | 229.3 | 308.2  |
| 2019--ICCV | [DSSINet](#DSSINet)                          | 216.9 | 302.4  |
| 2022--CVPR | [GauNet](#GauNet)(VGG-16)                    | 215.4 | 296.4  |
| 2019--CVPR | [SFCN](#CCWld)                               | 214.2 | 318.2  |
| 2019--CVPR | [CAN](#CAN)                                  | 212.2 | 243.7  |
| 2019--ICCV | [S-DCNet](#S-DCNet)                          | 204.2 | 301.3  |
| 2021--TPAMI| [LA-Batch](#LA-Batch) (backbone CSRNet)      | 203.0 | 230.6  |
| 2019--ICASSP| [ASD](#ASD)                                 | 196.2 | 270.9  |
| 2019--ICCV | [SPN+L2SM](#L2SM)                            | 188.4 | 315.3  |
| 2019--TIP  | [PaDNet](#PaDNet)                            | 185.8 | 278.3  |
| 2020--ICPR | [M-SFANet](#M-SFANet)                        | 162.33| 276.76 |
| 2021--AAAI | **[SASNet](#SASNet)**                        | **161.4** | **234.46** |

### WorldExpo'10
| Year-Conference/Journal | Method | S1 | S2 | S3 | S4 | S5 | Avg. |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 2015--CVPR | [Zhang 2015](#Zhang2015)              | 9.8  | 14.1  | 14.3  | 22.2 | 3.7  | 12.9 |
| 2016--CVPR | [MCNN](#MCNN)                         | 3.4  | 20.6  | 12.9  | 13.0 | 8.1  | 11.6 |
| 2017--ICIP | [MSCNN](#MSCNN)                       | 7.8  | 15.4  | 14.9  | 11.8 | 5.8  | 11.7 |
| 2017--ICCV | [ConvLSTM-nt](#ConvLSTM)              | 8.6  | 16.9  | 14.6  | 15.4 | 4.0  | 11.9 |
| 2017--ICCV | [ConvLSTM](#ConvLSTM)                 | 7.1  | 15.2  | 15.2  | 13.9 | 3.5  | 10.9 |
| 2017--ICCV | [Bidirectional   ConvLSTM](#ConvLSTM) | 6.8  | 14.5  | 14.9  | 13.5 | 3.1  | 10.6 |
| 2017--CVPR | [Switching CNN](#SCNN)                | 4.4  | 15.7  | 10.0  | 11.0 | 5.9  | 9.4  |
| 2017--ICCV | [CP-CNN](#CP-CNN)                     | 2.9  | 14.7  | 10.5  | 10.4 | 5.8  | 8.86 |
| 2018--AAAI | [TDF-CNN](#TDF-CNN)                   | 2.7  | 23.4  | 10.7  | 17.6 | 3.3  | 11.5 |
| 2018--CVPR | [IG-CNN](#IG-CNN)                     | 2.6  | 16.1  | 10.15 | 20.2 | 7.6  | 11.3 |
| 2018--TIP  | [BSAD](#BSAD)                         | 4.1  | 21.7  | 11.9  | 11.0 | 3.5  | 10.5 |
| 2018--ECCV | [ic-CNN](#ic-CNN)                     | 17.0 | 12.3  | 9.2   | 8.1  | 4.7  | 10.3 |
| 2018--CVPR | [DecideNet](#DecideNet)               | 2.0  | 13.14 | 8.9   | 17.4 | 4.75 | 9.23 |
| 2018--CVPR | [D-ConvNet-v1](#D-ConvNet)            | 1.9  | 12.1  | 20.7  | 8.3  | 2.6  | 9.1  |
| 2018--CVPR | [CSRNet](#CSR)                        | 2.9  | 11.5  | 8.6   | 16.6 | 3.4  | 8.6  |
| 2018--WACV | [SaCNN](#SaCNN)                       | 2.6  | 13.5  | 10.6  | 12.5 | 3.3  | 8.5  |
| 2018--ECCV | [SANet](#SANet)                       | 2.6  | 13.2  | 9.0   | 13.3 | 3.0  | 8.2  |
| 2018--IJCAI| [DRSAN](#DRSAN)                       | 2.6  | 11.8  | 10.3  | 10.4 | 3.7  | 7.76 |
| 2018--CVPR | [ACSCP](#ACSCP)                       | 2.8  | 14.05 | 9.6   | 8.1  | 2.9  | 7.5  |
| 2019--ICCV | [PGCNet](#PGCNet)                     | 2.5  | 12.7  | 8.4   | 13.7 | 3.2  | 8.1 |
| 2021--TPAMI| [LA-Batch](#LA-Batch)(backbone CSRNet)| 2.4  | 11.0  | 8.1   | 13.5 | 2.7  | 7.5  |
| 2019--CVPR | [TEDnet](#TEDnet)                     | 2.3  | 10.1  | 11.3  | 13.8 | 2.6  | 8.0  |
| 2019--CVPR | [PACNN](#PACNN)                       | 2.3  | 12.5  | 9.1   | 11.2 | 3.8  | 7.8  |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-bAttn-DME)     | 1.7   | 14.4  | 11.5 | 7.9  | 3.0  | 7.7 |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(AMG-attn-DME)      | 1.6   | 13.2  | 8.7  | 10.6    | 2.6 | 7.3 |
| 2019--CVPR | [CAN](#CAN)                           | 2.9  | 12.0  | 10.0  | 7.9  | 4.3  | 7.4  |
| 2019--CVPR | **[CAN](#CAN)(ECAN)**                 | 2.4  | **9.4** | 8.8 | 11.2 | 4.0 | 7.2 |
| 2019--ICCV | [DSSINet](#DSSINet)                   | 1.57 | 9.51 | 9.46 | 10.35 | 2.49 | 6.67 |
| 2020--ICPR | [M-SFANet](#M-SFANet)                 | 1.88 | 13.24 | 10.07 | 7.5 | 3.87 | 7.32 |
| 2020--CVPR | **[ASNet](#ASNet)**                   | 2.22 | 10.11 | 8.89 | **7.14** | 4.84 | 6.64 |
| 2021--AAAI | **[SASNet](#SASNet)**                 | **1.134** | 13.24 | **7.68** | 7.61 | **2.07** | **5.71** |


### UCSD

| Year-Conference/Journal | Method | MAE | MSE |
| --- | --- | --- | --- |
| 2015--CVPR | [Zhang 2015](#Zhang2015)                | 1.60 | 3.31 |
| 2016--ECCV | [Hydra-CNN](#Hydra-CNN)                 | 1.65 |  -   |
| 2016--ECCV | [CNN-Boosting](#CNN-Boosting)           | 1.10 |  -   |
| 2016--CVPR | [MCNN](#MCNN)                           | 1.07 | 1.35 |
| 2017--ICCV | [ConvLSTM-nt](#ConvLSTM)                | 1.73 | 3.52 |
| 2017--CVPR | [Switching CNN](#SCNN)                  | 1.62 | 2.10 |
| 2017--ICCV | [ConvLSTM](#ConvLSTM)                   | 1.30 | 1.79 |
| 2017--ICCV | [Bidirectional   ConvLSTM](#ConvLSTM)   | 1.13 | 1.43 |
| 2018--CVPR | [CSRNet](#CSR)                          | 1.16 | 1.47 |
| 2018--CVPR | [ACSCP](#ACSCP)                         | 1.04 | 1.35 |
| 2018--ECCV | [SANet](#SANet)                         | 1.02 | 1.29 |
| 2018--TIP  | [BSAD](#BSAD)                           | 1.00 | 1.40 |
| 2019--WACV | [SPN](#SPN)                             | 1.03 | 1.32 |
| 2019--ICCV | [SPANet+SANet](#SPANet)                 | 1.00 | 1.28 |
| 2019--CVPR | [ADCrowdNet](#ADCrowdNet)(DME)          | 0.98 | 1.25 |
| 2019--BMVC | [E3D](#E3D)                             | 0.93 | 1.17 |
| 2019--CVPR | [PACNN](#PACNN)                         | 0.89 | 1.18 |
| 2019--TIP  | **[PaDNet](#PaDNet)**                   | **0.85** | **1.06** |

### Mall

| Year-Conference/Journal | Method | MAE | MSE |
| --- | --- | --- | --- |
| 2012--BMVC | [Chen 2012](#Chen2012)                  | 3.15 | 15.7 |
| 2016--ECCV | [CNN-Boosting](#CNN-Boosting)           | 2.01 |  -   |
| 2017--ICCV | [ConvLSTM-nt](#ConvLSTM)                | 2.53 | 11.2 |
| 2017--ICCV | [ConvLSTM](#ConvLSTM)                   | 2.24 | 8.5  |
| 2017--ICCV | [Bidirectional   ConvLSTM](#ConvLSTM)   | 2.10 | 7.6  |
| 2018--CVPR | [DecideNet](#DecideNet)                 | 1.52 | 1.90 |
| 2018--IJCAI| [DRSAN](#DRSAN)                         | 1.72 | 2.1  |
| 2019--BMVC | [E3D](#E3D)                             | 1.64 | 2.13 |
| 2021--TPAMI| [LA-Batch](#LA-Batch) (backbone CSRNet) | 1.34 | 1.60 |
| 2019--WACV | **[SAAN](#SAAN)**                       | **1.28** | **1.68** |


## classification

### weakly/self/semi-supervised method
-

### domain adaption/generalization
- <a name="BLA"></a>**[BLA]** Bi-level Alignment for Cross-Domain Crowd Counting (**CVPR**) [[paper](https://arxiv.org/abs/2205.05844)][[code](https://github.com/Yankeegsj/BLA)]![GitHub stars](https://img.shields.io/github/stars/Yankeegsj/BLA.svg?logo=github&label=Stars)

    #### bi-level alignment: task-driven data alignment, fine-grained feature alignment(foreground and background).
    ### maybe the fine-grained feature alignment can be referred.
    ***
-


### segmentation assited method (background noise related)
- <a name="CUT"></a>**[CUT]** Segmentation Assisted U-shaped Multi-scale Transformer for Crowd Counting (**BMVC**) [[paper](https://www.researchgate.net/publication/364030579_Segmentation_Assisted_U-shaped_Multi-scale_Transformer_for_Crowd_Counting)]

    #### utilizes the good performance of transformer
    #### proposes a crowd u-transformer
    #### proposes a loss function to focus more on the foreground.
    ***
- <a name="HDNet"></a>**[HDNet]** HDNet: A Hierarchically Decoupled Network for Crowd Counting (**ICME**) [[paper](https://arxiv.org/abs/2212.05722)]

    #### decomposes the image counting task into background decomposing, foreground density decomposing, and introduces three interactions to compensate for the ignored correlation between the subtasks.
    ***
- <a name="RAN"></a>**[RAN]** Region-Aware Network: Model Human’s Top-Down Visual Perception Mechanism for Crowd Counting (**Neural Networks**) [[paper](https://arxiv.org/abs/2106.12163)]

    #### applies a top-down structure and tells the story well. I am not sure whether it completes the top-down structure that can allocate attention reasonably.
    ***
- <a name="SGANet"></a>**[SGANet]** Crowd Counting via Segmentation Guided Attention Networks and Curriculum Loss (**TITS**) [[paper](https://ieeexplore.ieee.org/document/9678116)]

    #### emmm, the revision is to replace vgg with inception-v3??? one more segmentation guided module and a curriculum loss are added......
    #### maybe the segmentation guided module is worth reading...
    ***
- <a name="HANet"></a>**[HANet]** Hybrid attention network based on progressive embedding scale-context for crowd counting (**Information Sciences**) [[paper](https://arxiv.org/abs/2106.02324)]

    #### apply paralleling spatial attention and channel attention to sovle the background noise and scaling problems simultaneously.
    ***
- <a name="CFANet"></a> **[CFANet]** Coarse- and Fine-grained Attention Network with Background-aware Loss for Crowd Density Map Estimation (**WACV**) [[paper](https://arxiv.org/abs/2011.03721)][[code](https://github.com/rongliangzi/MARUNet)]![GitHub stars](https://img.shields.io/github/stars/rongliangzi/MARUNet.svg?logo=github&label=Stars)

    #### coarse-to-fine-grained attention network to focus on crowd region and background aware loss to reduce the recognition.
    ***
- <a name="BSCC"></a> **[BSCC]** Understanding the impact of mistakes on background regions in crowd counting (**WACV**) [[paper](https://arxiv.org/abs/2003.13759)]

    #### analyze the mistaken prediction on the background in depth.
    #### add a simple segementation branch to alleviate the problem
    ***
- <a name="CRANet"></a> **[CRANet]** CRANet: Cascade Residual Attention Network for Crowd Counting (**ICME**) [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9428236)]

    #### proposes cascade residual attentoin to filter background noise.
    ***
- <a name="D2C"></a> **[D2C]** Decoupled Two-Stage Crowd Counting and Beyond (**TIP**) [[paper](https://ieeexplore.ieee.org/document/9347700)][[code](https://github.com/hustaia/Decoupled_Two-Stage_Counting)]![GitHub stars](https://img.shields.io/github/stars/hustaia/Decoupled_Two-stage_Counting.svg?logo=github&label=Stars)

    #### decouple the counting task into two stage, probability map estimation (can be called foreground/background segment maybe) and counting number estimation. the countor can learn from synthetic data.
    ***
- <a name="RRSP"></a> **[RRSP]** Residual Regression with Semantic Prior for Crowd Counting (**CVPR**) [[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wan_Residual_Regression_With_Semantic_Prior_for_Crowd_Counting_CVPR_2019_paper.pdf)][[code](https://github.com/jia-wan/ResidualRegression-pytorch)] ![GitHub stars](https://img.shields.io/github/stars/jia-wan/ResidualRegression-pytorch.svg?logo=github&label=Stars)

### reasoning based method
- <a name="TopoCount"></a> **[TopoCount]**  Localization in the Crowd with Topological Constraints (**AAAI**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/16170)][[code](https://github.com/ShahiraAbousamra/TopoCount)]![GitHub stars](https://img.shields.io/github/stars/ShahiraAbousamra/TopoCount.svg?logo=github&label=Stars)

    #### uses topological reasoning to avoid the wrong clustered localization results.
    ***

### scale-related method
- <a name="LoViTCrowd"></a>**[LoViTCrowd]** Improving Local Features with Relevant Spatial Information by Vision Transformer for Crowd Counting (**BMVC**) [[paper](https://bmvc2022.mpi-inf.mpg.de/0729.pdf)] [[code](https://github.com/nguyen1312/LoViTCrowd)]![GitHub stars](https://img.shields.io/github/stars/nguyen1312/LoViTCrowd.svg?logo=github&label=Stars)

    #### an application of ViT, and then?
    ***

### multi-modal method
- <a name="MSDTrans"></a>**[MSDTrans]** RGB-T Multi-Modal Crowd Counting Based on Transformer (**BMVC**)[[paper](https://arxiv.org/abs/2301.03033)] [[code](https://github.com/liuzywen/RGBTCC)]![GitHub stars](https://img.shields.io/github/stars/liuzywen/RGBTCC.svg?logo=github&label=Stars)

    #### perform RGB-IR crowd counting with transformer...multi-modal fusion
    ***

### class-agnostic counting method
- <a name="SPDCN"></a>**[SPDCN]** Scale-Prior Deformable Convolution for Exemplar-Guided Class-Agnostic Counting (**BMVC**) [[paper](https://bmvc2022.mpi-inf.mpg.de/0313.pdf)]

    #### solves the scaling problem in class-agnostic counting with deformable convolution and scale-sensitive loss function.
    ***

### multi-view crowd counting
-

### crowd localization
- <a name="CLTR"></a>**[CLTR]** An End-to-End Transformer Model for Crowd Localization (**ECCV**) [[paper](https://arxiv.org/abs/2202.13065)] [[code](https://github.com/dk-liang/CLTR)]![GitHub stars](https://img.shields.io/github/stars/dk-liang/CLTR.svg?logo=github&label=Stars)[[project](https://dk-liang.github.io/CLTR/)]

    #### apply set prediction paradigm for the crowd localization task with KMO based macher.
    ***
-

### point supervision
- <a name="PSODC"></a> **[PSODC]** A Self-Training Approach for Point-Supervised Object Detection and Counting in Crowds (**TIP**) [[paper](https://arxiv.org/abs/2007.12831)][[code](https://github.com/WangyiNTU/Point-supervised-crowd-detection)]![GitHub stars](https://img.shields.io/github/stars/WangyiNTU/Point-supervised-crowd-detection.svg?logo=github&label=Stars)

    #### a self-training method for object detection and crwod counting with point annotations.
    ***
-

### other method
- <a name="DC"></a>**[DC]** Discrete-Constrained Regression for Local Counting Models (**ECCV**) [[paper](https://arxiv.org/abs/2207.09865)]

    #### finds the reasons why classification methods show better performance than regression methods: inaccurate dot annotation and inappropriate gaussian kernel.
    #### futhermore, proposes a discrete regression method to avoid these problems.
    ***
- Redesigning Multi-Scale Neural Network for Crowd Counting [[paper](https://arxiv.org/abs/2208.02894)][[code](https://github.com/ZPDu/Redesigning-Multi-Scale-Neural-Network-for-Crowd-Counting)]![GitHub stars](https://img.shields.io/github/stars/ZPDu/Redesigning-Multi-Scale-Neural-Network-for-Crowd-Counting.svg?logo=github&label=Stars)

    #### designs many complicated structures to solve the scaling problem
    #### merge multi-scale feature, expert scheme, soft gating and loss fuc. kind of interesting and maybe can be reffered.
    ***

### survey
- Revisiting Crowd Counting: State-of-the-art, Trends, and Future Perspectives (**Image and Vision Computing**) [[paper](https://arxiv.org/abs/2209.07271)]

    #### A survey paper, relatively new, maybe can relief my work.
    ***


### mapping and counting: a new trial