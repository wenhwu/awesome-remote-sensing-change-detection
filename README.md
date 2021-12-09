# Awesome Remote Sensing Change Detection [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

List of datasets, codes, and contests related to remote sensing change detection.

![ReCNN](/2018.recurrent&#32;convolutional&#32;neural&#32;network.jpg)

## 1 Dateset

### 1.1 Multispectral

#### With label
- 2021.[HTCD dataset](https://github.com/ShaoRuizhe/SUNet-change_detection)   
The HTCD dataset, a new Satellite-UAV heterogeneous image data set, was built using the satellite images from [Google Earth](https://www.google.com/earth/) and UAV images from [Open Aerial Map](https://map.openaerialmap.org/). The size of the satellite image is 11 K×15 K pixels. While the UAV image is consisted of 15 image blocks, in total 1.38 M×1.04 M pixels. The ground resolutions of them are 0.5971 m and 7.465 cm, respectively. Images and labels are all stored in GeoTiff format with location information, for the convenience of further analysis and research. Paper: [Shao et al.2021](https://www.mdpi.com/2072-4292/13/18/3750/htm)

- 2021.[Multi-modal Supervised Change Detection Data](https://github.com/PatrickTUM/multimodalCD_ISPRS21)   
Sentinel-1 SAR data were provided on the basis of [OSCD dataset](https://ieee-dataport.org/open-access/oscd-onera-satellite-change-detection) for multimodal supervised change detection (SAR-SAR CD or Optical-SAR multi-modal CD). Paper: [Ebel et al.2021](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIII-B3-2021/243/2021/isprs-archives-XLIII-B3-2021-243-2021.pdf)

- 2021.[S2Looking](https://github.com/AnonymousForACMMM/Dataset)   
S2Looking, a building change detection dataset that contains large-scale side-looking satellite images captured at varying off-nadir angles. It consists of 5000 registered bitemporal image pairs (size of 1024*1024, 0.5 ~ 0.8 m/pixel) of rural areas throughout the world and more than 65,920 annotated change instances. It provides two label maps to separately indicate the newly built and demolished building regions for each sample in the dataset. Paper: [Shen et al.2021](https://arxiv.org/abs/2107.09244)

- 2021.[SYSU-CD](https://github.com/liumency/SYSU-CD)   
The dataset contains 20000 pairs of 0.5-m aerial images of size 256×256 taken between the years 2007 and 2014 in Hong Kong.The main types of changes in the dataset include: (a) newly built urban buildings; (b) suburban dilation; (c) groundwork before construction; (d) change of vegetation; (e) road expansion; (f) sea construction. Paper: [Shi et al.2021](https://ieeexplore.ieee.org/document/9467555)

- 2021.[**Sentinel-2 Multitemporal Cities Pairs (S2MTCP) dataset**](https://zenodo.org/record/4280482#.YBBCX-j7RhE)   
The S2MTCP dataset contains N = 1520 image pairs, spread over all inhabited continents, with the highest concentration of image pairs in North-America, Europe, and Asia. Bands with a spatial resolution smaller than 10 m are resampled to 10 m and images are cropped to approximately 600x600 pixels. It was created for self-supervised training. Paper: [Leenstra et al.2021](https://arxiv.org/abs/2101.08122)

- 2020.**Hi-UCD**   
Hi-UCD focuses on urban changes and uses ultra-high resolution images to construct multi-temporal semantic changes to achieve refined change detection. The study area of Hi-UCD is a part of Tallinn, the capital of Estonia, with an area of 30km2. There are 359 image pairs in 2017-2018, 386 pairs in 2018-2019, and 548 pairs in 2017-2019, including images, semantic maps, and change maps at different times. Each image has a size of 1024 x 1024 and a spatial resolution of 0.1 m. There are 9 types of objects, including natural objects (water, grassland, woodland, bare land), artificial objects (Building,greenhouse, road, bridge), and others (change-related), basically include all types of urbanland cover in Estonia. Paper: [Tian et al.2020](https://arxiv.org/abs/2011.03247)

- 2020.[**DSIFN Dataset**](https://github.com/GeoZcx/A-deeply-supervised-image-fusion-network-for-change-detection-in-remote-sensing-images/tree/master/dataset)   
The dataset is manually collected from Google Earth. It consists of six large bi-temporal high resolution images covering six cities (i.e., Beijing, Chengdu, Shenzhen, Chongqing, Wuhan, Xian) in China. The five large image-pairs (i.e., Beijing, Chengdu, Shenzhen, Chongqing, Wuhan) are clipped into 394 subimage pairs with sizes of 512×512. After data augmentation, a collection of 3940 bi-temporal image pairs is acquired. Xian image pair is clipped into 48 image pairs for model testing. There are 3600 image pairs in the training dataset, 340 image paris in the validation dataset, and 48 image pairs in the test dataset. Paper: [Zhang et al.2020](https://www.sciencedirect.com/science/article/abs/pii/S0924271620301532)

- 2020.[**SEmantic Change detectiON Dataset (SECOND)**](http://www.captain-whu.com/PROJECT/SCD/)   
SECOND, a well-annotated semantic change detection dataset, which collects 4662 pairs of aerial images from several platforms and sensors. These pairs of images are distributed over the cities such as Hangzhou, Chengdu, and Shanghai. Each image has size 512 x 512 and is annotated at the pixel level. SECOND focus on 6 main land-cover classes, i.e. , non-vegetated ground surface, tree, low vegetation, water, buildings, and playgrounds, that are frequently involved in natural and man-made geographical changes. Paper: [Yang et al.2020](https://arxiv.org/abs/2010.05687)


- 2020.[**Google Dataset**](https://github.com/daifeng2016/Change-Detection-Dataset-for-High-Resolution-Satellite-Imagery)   
The images were acquired during the periods between 2006 and 2019, covering the suburb areas of Guangzhou City, China. To facilitate image pair generation, Google Earth service through the [BIGEMAP](http://www.bigemap.com) software was adopted to collect 19 season-varying VHR images pairs with three bands of red, green, and blue, a spatial resolution of 0.55 m, and the size ranging from 1006×1168 pixels to 4936×5224 pixels. The annotation is focused on buildings. Paper: [Peng et al.2020](https://ieeexplore.ieee.org/document/9161009)

- 2020.[**LEVIR building Change Detection (LEVIR-CD) Dataset**](https://justchenhao.github.io/LEVIR/)   
LEVIR-CD consists of 637 very high-resolution (VHR, 0.5m/pixel) Google Earth image patch pairs with a size of 1024 × 1024 pixels. These bitemporal images with time span of 5 to 14 years have significant land-use changes, especially the construction growth. LEVIR-CD covers various types of buildings, such as villa residences, tall apartments, small garages and large warehouses. The fully annotated LEVIR-CD contains a total of 31,333 individual change building instances. LEVIR-CD+ can be found in this [page](https://github.com/AnonymousForACMMM/Dataset). Paper: [Chen et al.2020](https://www.mdpi.com/2072-4292/12/10/1662)

- 2019.[**High Resolution Semantic Change Detection (HRSCD) Dataset**](https://ieee-dataport.org/open-access/hrscd-high-resolution-semantic-change-detection-dataset)   
This dataset contains 291 coregistered image pairs of RGB aerial images from IGS's BD ORTHO database. Pixel-level change and land cover annotations are provided, generated by rasterizing Urban Atlas 2006, Urban Atlas 2012, and Urban Atlas Change 2006-2012 maps. Paper: [Daudt et al.2019](https://www.sciencedirect.com/science/article/pii/S1077314219300992)
  
- 2019.[**Wuhan multi-temperature scene (MtS-WH) Dataset**](http://sigma.whu.edu.cn/newspage.php?q=2019_03_26)   
The dataset is mainly used for theoretical research and verification of scene change detection methods. It consists of two large-size VHR images, which have a size of 7200x6000 and are respectively acquired by IKONOS sensors in Feb 2002 and Jun 2009. The images cover the Hanyang District, Wuhan City, China and contain 4 spectral bands (Blue, Green, Red, and Near-Infrared). The spatial resolution of the images is 1m after fusion of the pan and multispectral images by the Gram–Schmidt algorithm. For a discussion of this dataset, please refer to [#3](https://github.com/wenhwu/awesome-remote-sensing-change-detection/issues/3). Paper: [Wu et al.2017](https://ieeexplore.ieee.org/document/7817860)

- 2018.[**WHU Building change detection Dataset**](https://study.rsgis.whu.edu.cn/pages/download/building_dataset.html)   
The dataset contains two aerial images (0.2m/pixel, 15354×32507) and provides a change vector, a change raster map, and two corresponding building vectors of these two aerial images. Paper: [Ji et al.2018](https://ieeexplore.ieee.org/document/8444434)

- 2018.[**Synthetic images and real season-varying remote sensing images**](https://drive.google.com/file/d/1GX656JqqOyBi_Ef0w65kDGVto-nHrNs9/edit)   
This dataset has three types: synthetic images without objects relative shift, synthetic images with small relative shift of objects, real season-varying remote sensing images (obtained by Google Earth). The real season-varying remote sensing images have 16000 image sets with image size 256x256 pixels (10000 train sets and 3000 test and validation sets) and a spatial resolution of 3 to 100 cm/px. For a discussion of this dataset, please refer to [#5](https://github.com/wenhwu/awesome-remote-sensing-change-detection/issues/5). Paper: [Lebedev et al.2018](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLII-2/565/2018/isprs-archives-XLII-2-565-2018.pdf)

- 2018.[**Onera Satellite Change Detection Dataset**](https://ieee-dataport.org/open-access/oscd-onera-satellite-change-detection)   
This dataset addresses the issue of detecting changes between satellite images from different dates. It comprises 24 pairs of multispectral images taken from the Sentinel-2 satellites between 2015 and 2018. Locations are picked all over the world, in Brazil, USA, Europe, Middle-East and Asia. For each location, registered pairs of 13-band multispectral satellite images obtained by the Sentinel-2 satellites are provided. Images vary in spatial resolution between 10m, 20m, and 60m. Paper: [Daudt et al.2018](https://ieeexplore.ieee.org/document/8518015)

- 2011.[**The Aerial Imagery Change Detection (AICD) dataset**](https://computervisiononline.com/dataset/1105138664)   
This dataset contains synthetic aerial images with artificial changes generated with a rendering engine. It contains 1000 pairs of 800x600 images, each pair consisting of one reference image and one test image, and the 1000 corresponding 800x600 ground truth masks. Paper: [Bourdis et al.2011](https://ieeexplore.ieee.org/document/6050150)

- 2008.[**SZTAKI AirChange Benchmark set**](http://web.eee.sztaki.hu/remotesensing/airchange_benchmark.html)   
This dataset contains 13 aerial image pairs of size 952x640 and resolution 1.5m/pixel and binary change masks (drawn by hand). Each record contains a pair of preliminary registered input images and a mask of the 'relevant' changes. The input images are taken with 5, 7 resp. 23 years of time differences. During the generation of the change mask, we have considered the following differences as relevant changes: (a) new built-up regions (b) building operations (c) planting of large group of trees (d) fresh plow-land (e) groundwork before building over. Note that the ground truth does NOT contain change classification, only binary change-no change decision for each pixel. Paper: [Benedek et al.2008](https://ieeexplore.ieee.org/document/5169964)

#### Without label

- [Planet Disaster Datasets](https://www.planet.com/disasterdata/datasets/)   
Planet will make PlanetScope imagery available to the public during a select disaster event.

- [DigitalGlobe's Open Data Program](https://www.digitalglobe.com/opendata/all-events)   
 DigitalGlobe will release open imagery (worldview-3 or other) for select sudden onset major crisis events, including pre-event imagery, post-event imagery, and a crowdsourced damage assessment.

- [French National Institute of Geographical and Forest Information (IGN),BD ORTHO](http://professionnels.ign.fr/bdortho)   
The datasets are mosaics of aerial images taken by the French National Institute of Geographical and Forest Information (IGN). They come from a database named BD ORTHO which contains orthorectified aerial images of several regions of France from different years at a resolution of 20 cm or 50 cm per pixel. 

- [LINZ DATA SERVICE](https://data.linz.govt.nz/)   
The New Zealand Land Information Services website provides multi-temporal aerial images of some New Zealand cities, all of which have a resolution of over 1m.

- [USGS EarthExplorer](https://earthexplorer.usgs.gov)   
An epic level database, which can provide multi-temporal，multi-sensor and multi-resolution data.

### 1.2 Hyperspectral

- 2018.[Hyperspectral Change Detection Dataset](https://citius.usc.es/investigacion/datasets/hyperspectral-change-detection-dataset)   
This dataset can be used to perform change detection techniques in multi-temporal hyperspectral images. It includes two different hyperspectral scenes from the AVIRIS sensor: The Santa Barbara scene, taken on the years 2013 and 2014 with the AVIRIS sensor over the Santa Barbara region (California) whose spatial dimensions are 984 x 740 pixels and includes 224 spectral bands. The Bay Area scene, taken on the years 2013 and 2015 with the AVIRIS sensor surrounding the city of Patterson (California) whose spatial dimensions are 600 x 500 pixels and includes 224 spectral bands.
It also includes a hyperspectral scene from the HYPERION sensor: The Hermiston city scene, taken on the years 2004 and 2007 with the HYPERION sensor over the Hermiston City area (Oregon) whose spatial dimensions are 390 x 200 pixels and includes 242 spectral bands. 5 types of changes related to crop transitions are identified in this scene. Paper: [López-Fandiño et al.2018](https://ieeexplore.ieee.org/document/8518338)

- 2018.[GETNET](https://drive.google.com/file/d/1cWy6KqE0rymSk5-ytqr7wM1yLMKLukfP/view)   
This dataset has two hyperspectral images, which were acquired on May 3, 2013, and December 31, 2013, respectively in Jiangsu province, China. It has a size of 463×241 pixels, with 198 bands available after noisy band removal. In the ground-truth map, white pixels represent changed portions and black pixels mean unchanged parts. Paper: [Wang et al.2018](https://ieeexplore.ieee.org/document/8418840/?denied=)

### 1.3 3D
- 2021.[URB3DCD](https://ieee-dataport.org/open-access/urb3dcd-urban-point-clouds-simulated-dataset-3d-change-detection)   
The dataset is based on LoD2 models of [the first and second districts of Lyon](https://geo.data.gouv.fr/datasets/0731989349742867f8e659b4d70b707612bece89), France. To conduct fair qualitative and quantitative evaluation of point clouds change detection techniques. This first version of the dataset is composed of point clouds at a challenging low resolution of around 0.5 points/meter². Paper: [de Gélis et al.2021](https://www.mdpi.com/2072-4292/13/13/2629)

## 2 Code

### 2.1 Multispectral

#### 2.1.1 Traditional Method

- 2019.[Bobholamovic/ChangeDetectionToolbox](https://github.com/Bobholamovic/ChangeDetectionToolbox)

- 2019.[Canty M J. Image Analysis, Classification and Change Detection in Remote Sensing (Fourth Revised Edition)](https://github.com/mortcanty/CRC4Docker)

- 2017.[Canty M J. Change Detection with Google Earth Engine Imagery](https://github.com/mortcanty/earthengine)

- 2014.[Canty M J. Image Analysis, Classification and Change Detection in Remote Sensing (Third Revised Edition)](https://github.com/mortcanty/CRCPython)

- [Zhu Z, Woodcock C E, et al. Algorithm developed for Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data](https://github.com/GERSL/CCDC)

- Implementation of " [2009.Celik T. Unsupervised change detection in satellite images using principal component analysis and k-means clustering](https://ieeexplore.ieee.org/abstract/document/5196726/) ".  
[Matlab](https://github.com/rulixiang/ChangeDetectionPCAKmeans), [Python](https://github.com/abhijeet3922/Change-Detection-in-Satellite-Imagery)

- 2007.[Nielsen A A.The Regularized Iteratively Reweighted Multivariate Alteration Detection (IR-MAD)](http://people.compute.dtu.dk/alan/software.html)

#### 2.1.2 Deep Learning (Only the last three years are shown)
- 2021.[Shi Q, Liu M, Li S, et al. A Deeply Supervised Attention Metric-Based Network and an Open Aerial Image Dataset for Remote Sensing Change Detection](https://github.com/liumency/DSAMNet)

- 2021.[Shao R, Du C, Chen H, et al. SUNet: Change Detection for Heterogeneous Remote Sensing Images from Satellite and UAV Using a Dual-Channel Fully Convolution Network](https://github.com/ShaoRuizhe/SUNet-change_detection)

- 2021.[Diakogiannis F I, Waldner F, Caccetta P. Looking for change? Roll the Dice and demand Attention](https://github.com/feevos/ceecnet)

- 2021.[Papadomanolaki M, Vakalopoulou M, Karantzalos K. A Deep Multi-Task Learning Framework Coupling Semantic Segmentation and Fully Convolutional LSTM Networks for Urban Change Detection](https://github.com/mpapadomanolaki/multi-task-L-UNet)

- 2021.[Zheng Z, Zhong Y, Wang J, et al. Building damage assessment for rapid disaster response with a deep object-based semantic change detection framework:
from natural disasters to man-made disasters](https://github.com/Z-Zheng/ChangeOS)

- 2021.[likyoo/change_detection.pytorch](https://github.com/likyoo/change_detection.pytorch): Deep learning models for change detection of remote sensing images

- 2021.[Xu J, Luo C, Chen X, et al. Remote Sensing Change Detection Based on Multidirectional Adaptive Feature Fusion and Perceptual Similarity](https://github.com/wzjialang/MFPNet)

- 2021.[geoyee/PdRSCD](https://github.com/geoyee/PdRSCD): Remote sensing change detection tool based on PaddlePaddle

- 2021.[Zhang H, Lin M, Yang G, et al. ESCNet: An End-to-End Superpixel-Enhanced Change Detection Network for Very-High-Resolution Remote Sensing Images](https://github.com/Bobholamovic/ESCNet)

- 2021.[Mañas O, Lacoste A, Giro-i-Nieto X, et al. Seasonal Contrast: Unsupervised Pre-Training from Uncurated Remote Sensing Data](https://github.com/ElementAI/seasonal-contrast)

- 2021.[Zheng Z, Ma A, Zhang L, et al. Change is Everywhere: Single-Temporal Supervised Object Change Detection for High Spatial Resolution Remote Sensing Imagery](https://github.com/Z-Zheng/ChangeStar)

- 2021.[Liu M, Shi Q, Marinoni A, et al. Super-resolution-based Change Detection Network with Stacked Attention Module for Images with Different Resolutions](https://github.com/liumency/SRCDNet)

- 2021.[Xu Q, Chen K, Zhou G, et al. Change Capsule Network for Optical Remote Sensing Image Change Detection](https://github.com/xuquanfu/capsule_change_detection)

- 2021.[Chen H, Qi Z, Shi Z. Remote Sensing Image Change Detection with Transformers](https://github.com/justchenhao/BIT_CD)   

- 2021.[Chen H, Li W, Shi Z, .Adversarial Instance Augmentation for Building Change Detection in Remote Sensing Images](https://github.com/justchenhao/IAug_CDNet)

- 2021.[Fang S, Li K, Shao J, et al. SNUNet-CD: A Densely Connected Siamese Network for Change Detection of VHR Images](https://github.com/likyoo/Siam-NestedUNet)

- 2020.[I-Hope-Peace/ChangeDetectionRepository](https://github.com/I-Hope-Peace/ChangeDetectionRepository)

- 2020.[Zhang C, Yue P, Tapete D, et al. A deeply supervised image fusion network for change detection in high resolution bi-temporal remote sensing images](https://github.com/GeoZcx/A-deeply-supervised-image-fusion-network-for-change-detection-in-remote-sensing-images)
  
- 2020.[Chen H, Shi Z. A Spatial-Temporal Attention-Based Method and a New Dataset for Remote Sensing Image Change Detection](https://github.com/justchenhao/STANet)

- 2020.[Zhang M, Shi W. A Feature Difference Convolutional Neural Network-Based Change Detection Method](https://github.com/MinZHANG-WHU/FDCNN)

- 2020.[llu025/Heterogeneous_CD](https://github.com/llu025/Heterogeneous_CD)
  
- 2020.[neverstoplearn/remote_sensing_change_detection](https://github.com/neverstoplearn/remote_sensing_change_detection)
  
- 2020.[Chen J, Yuan Z, Peng J, et al. DASNet: Dual attentive fully convolutional siamese networks for change detection of high resolution satellite images](https://github.com/lehaifeng/DASNet)

- 2019.[Saha S et al. Unsupervised deep change vector analysis for multiple-change detection in VHR images](https://github.com/sudipansaha/dcvaVHROptical)

- 2019.[Papadomanolaki M, Verma S, Vakalopoulou M, et al. Detecting Urban Changes with Recurrent Neural Networks from Multitemporal Sentinel-2 Data](https://github.com/granularai/ChangeDetection)

- 2019.[Du B, Ru L, Wu C, et al. Deep Slow Feature Analysis Network (DSFANet)](https://github.com/rulixiang/DSFANet)

- 2019.[Peng D, Zhang Y, Guan H. End-to-End Change Detection for High Resolution Satellite Images Using Improved UNet++](https://github.com/daifeng2016/End-to-end-CD-for-VHR-satellite-image)

### 2.2 SAR

- 2019.[Gao F, Wang X, Gao Y, et al. Sea ice change detection in SAR images based on convolutional-wavelet neural networks (Matlab)](https://github.com/summitgao/SAR_Change_Detection_CWNN)

- 2019.[Gao Y, Gao F, Dong J, et al. Transferred deep learning for sea ice change detection from synthetic-aperture radar images (Matlab)](https://github.com/summitgao/SAR-Change-Detection-MLFN)
  
- 2015.[Conradsen K, Nielsen A A, Skriver H, et al. Change detection in polarimetric SAR Data (Python)](https://github.com/fouronnes/SAR-change-detection)

## 3.Contest
- [2021“昇腾杯”遥感影像智能处理算法大赛-耕地建筑物变化检测](http://rsipac.whu.edu.cn/subject_two)*(Wuhan University, Sep 2021)*   
通过前后两时相的遥感影像，提取出地物发生变化的像元并赋予变化标签。 依据所述地物变化标准，以耕地-建筑/动土的像素级变化检测为目标。数据为1-2米分辨率光学遥感影像，6000+张遥感影像变化检测样本数据(按512 X 512大小折算)。标签格式为单通道的png，每个像素的标签值由一个数值表示， 使用‘uint8’数据类型存储，该数值表示是否为变化，“0”代表未变化，“1”代表变化。     

- [2021 遥感图像智能解译技术挑战赛-建筑物变化检测](https://captain-whu.github.io/PRCV2021_RS/index.html)*(Wuhan University, PIESAT, Aug 2021)*   
本竞赛数据集主要包含涉及建筑物的地物变化。全部图像数据共10000对（训练集：6000对图像，验证集：2000对图像，测试样本：2000对图像），尺寸为512 x 512，主要分布于北京、上海、广州以及杭州等城市。部分数据源自[SECOND](http://www.captain-whu.com/PROJECT/SCD/)数据集。第三名解决方案详见[likyoo/PRCV2021_ChangeDetection_Top3](https://github.com/likyoo/PRCV2021_ChangeDetection_Top3)。

- [2021 第五届“中科星图杯”国际高分遥感图像解译大赛-高分辨率可见光图像中建筑物普查与变化检测](http://gaofen-challenge.com/challenge) *(Aircas,et al. Aug 2021)*    
高分二号、吉林一号光学数据，分辨率优于1m。每幅图像对建筑物进行像素级标注，同一时相数据对变化的建筑物区域进行像素级标注。建筑物提取类别：建筑物和背景，变化检测类别：变化的建筑区域和非变化的建筑区域。

- [2021 慧眼“天智杯”人工智能挑战赛-可见光建筑智能变化检测](https://www.rsaicp.com/portal/contestDetail?id=1&tab=rule) *(北京市遥感信息研究所，中国科学院人工智能创新研究院. Jun 2021)*    
每组数据包含前时相遥感图像，后时相遥感图像以及对应的建筑变化标签图。影像格式为png，包含R、G、B三个波段，影像尺寸为1024 X 1024像素，分辨率为0.5~0.7米。标签图与图像等大，其中 (0,0,0) 代表没有建筑变化，(0,0,255) 代表建筑增加，(255,0,0) 代表建筑减少。

- [2021 DynamicEarthNet Challenge](http://www.classic.grss-ieee.org/earthvision2021/challenge.html) *(TUM, DLR, panet, Mar 2021)*    
The challenge consists of two tracks (**Unsupervised Binary Land Cover Change Detection** and **Weakly-Supervised Multi-Class Change Detection**) in which participants are tasked to detect multi-temporal changes with few or no training labels. 

- [2021 IEEE GRSS Data Fusion Contest: Track MSD (Multitemporal Semantic Change Detection)](https://www.grss-ieee.org/community/technical-committees/2021-ieee-grss-data-fusion-contest-track-msd/) *(GRSS, Microsoft, Jan 2021)*   
The task of Track MSD is to create bitemporal high resolution land cover maps using only low-resolution and noisy land cover labels for training. Such a scenario is often encountered around the world, as the proliferation of new sensors with either high spatial resolution (submeter) or high temporal resolution (weekly or even daily) remains unmatched by equally rich label data. Instead, detecting change would have to rely on the analysis of a sequence of input images in an unsupervised manner or with aid of weak, noisy, and outdated labels.

- [**SpaceNet 7: Multi-Temporal Urban Development Challenge**](https://medium.com/the-downlinq/the-spacenet-7-multi-temporal-urban-development-challenge-dataset-release-9e6e5f65c8d5) *(CosmiQ Works, Planet, Aug 2020)*   
In this challenge, participants will identify and track buildings in satellite imagery time series collected over rapidly urbanizing areas. The competition centers around a new open source dataset of Planet satellite imagery mosaics, which will include 24 images (one per month) covering ~100 unique geographies. The dataset will comprise 40,000 km2 of imagery and exhaustive polygon labels of building footprints in the imagery, totaling over 3M individual annotations. Challenge participants will be asked to track building construction over time, thereby directly assessing urbanization.

- [**商汤科技首届AI遥感解译大赛-变化检测赛道**](https://rs.sensetime.com/competition/index.html#/info) *(SenseTime, Aug 2020)*   
数据集：4662组，分辨率：0.5~3m，规格：512*512，变化类型为6种主要土地性质之间的相互转化：水体、地面、低矮植被、树木、建筑物、运动场。每组数据中，前后时相的两张图片各自对应一张标注图，表示发生变化的区域以及该图片变化区域内各时期的土地性质。第一名的解决方案详见 [LiheYoung/SenseEarth2020-ChangeDetection](https://github.com/LiheYoung/SenseEarth2020-ChangeDetection)。

- [**xView 2 Building Damage Asessment Challenge**](https://xview2.org) *(DIUx, Nov 2019)*     
550k building footprints & 4 damage scale categories, 20 global locations and 7 disaster types (wildfire, landslides, dam collapses, volcanic eruptions, earthquakes/tsunamis, wind, flooding), Worldview-3 imagery (0.3m res.), pre-trained baseline model. Paper: [Gupta et al. 2019](https://arxiv.org/abs/1911.09296)

- [**遥感图像稀疏表征与智能分析竞赛-变化检测赛道**](http://rscup.bjxintong.com.cn/#/theme/4) *(Wuhan University,et al. Jul 2019)*   
本项竞赛以光学遥感图像为处理对象，参赛队伍使用主办方提供的遥感图像进行建筑物变化检测，主办方根据评分标准对变化检测结果进行综合评价。竞赛中将提供两个不同时间获取的大尺度高分辨率遥感图像（包含蓝、绿、红和近红外四个波段），以及图像中变化区域的二值化标注数据集。

- [**广东政务数据创新大赛—智能算法赛**](https://tianchi.aliyun.com/competition/entrance/231615/introduction) *(Alibaba,et al. Nov 2017)*    
使用2015年和2017年分别获取到的广东省某地的Quickbird卫星影像（包含蓝、绿、红和近红外四个波段），识别出两年之间新增的人工地上建筑物（不包括道路）。获胜团队的解决方案可以在[天池](https://tianchi.aliyun.com/forum/postDetail?postId=3527)官网上找到。

## Reference

- [chrieke/awesome-satellite-imagery-datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [Zhang Bin's Blog. Remote Sensing Datasets](https://zhangbin0917.github.io/2018/06/12/%E9%81%A5%E6%84%9F%E6%95%B0%E6%8D%AE%E9%9B%86/)
- [MinZHANG-WHU/Change-Detection-Review](https://github.com/MinZHANG-WHU/Change-Detection-Review)
- The picture of this page is from [Mou L et al. 2018](https://ieeexplore.ieee.org/document/8541102)
