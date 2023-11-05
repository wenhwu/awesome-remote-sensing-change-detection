# <p align=center>`Awesome Remote Sensing Change Detection`</p>
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) [![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)

List of datasets, codes, and contests related to remote sensing change detection.

# Contents

- [Dateset](#dateset)
  - [Multispectral](#multispectral)
    - [With Label](#with-label)
    - [Without Label](#without-label)
  - [Hyperspectral](#hyperspectral)
  - [3D](#3d)
- [Code](#code)
  - [Multispectral](#multispectral-1)
    - [Traditional Method](#traditional-method)
    - [Deep Learning](#deep-learning)
      - [2D](#2d)
      - [3D](#3d-1)
  - [SAR](#sar)
  - [Hyperspectral](#hyperspectral-1)
- [Contest](#contest)
- [Reference](#reference)

# Dateset

## Multispectral

### With Label   

- 2023.[SMARS (Simulated Multimodal Aerial Remote Sensing) dataset](https://www.sciencedirect.com/science/article/pii/S092427162300254X?dgcid=rss_sd_all)      
SMARS is a large-scale synthetic dataset, comprising pairs of scenarios simulating urban changes, designed for training and validating change detection applications, as well as urban segmentation and building extraction tasks. The dataset simulates the terrains of two European cities: Paris and Venice, generating scenario pairs named SParis and SVenice, each accompanied by ortho-images and Digital Surface Models (DSMs). Changes between the before and after scenarios are simulated, with the latter having more buildings, less green space, and some simulated demolished buildings. To enhance similarity with real data, input images are further processed into ortho-photos and digital elevation models through a standard photogrammetric process, including different lighting conditions and other effects, such as blurred building boundaries. Reference ground truth maps are directly used for training and validation of change detection, building extraction, and urban segmentation tasks. The data is rendered at two Ground Sampling Distances (GSDs) of 30cm and 50cm. Each tile, from left to right, includes: optical image, DSM, semantic and building masks. For change detection, the difference between two events is used as the ground truth. Paper: [Reyes et al., 2023](https://www.sciencedirect.com/science/article/pii/S092427162300254X)

- 2023.[**HRCUS-CD (High-Resolution Complex Urban Scene Change Detection)**](https://github.com/zjd1836/AERNet)   
The proposed High-Resolution Complex Urban Scene Change Detection (HRCUS-CD) dataset consists of 11,388 pairs of cropped high-resolution remote sensing images. The image size is 256 × 256 pixels with a resolution of 0.5 meters. The dataset includes over 12,000 annotated instances of changes. The data was collected in Zhuhai, China. It contains two main acquisition areas from two image sources: the first is mainly the urban built-up area, with a time span from 2019 to 2022. Considering the short time interval and the fact that this area is mostly built-up, the building changes’ areas are small. The second area spans from 2010 to 2018, and contains farmland and mountains, with a small number of old civil houses and buildings in the early period, and the area of building change is large later. These two types of high-resolution RSIs focus on built-up areas and new urban areas. Paper: [Zhang et al., 2023](https://ieeexplore.ieee.org/document/10209204)

- 2023.[**GVLM**](https://github.com/zxk688/GVLM)   
The Global Very-High-Resolution Landslide Mapping (GVLM) dataset is the first large-scale and open-source VHR landslide mapping dataset. It includes 
 17 bitemporal very-high-resolution imagery pairs with a spatial resolution of 0.59 m acquired via Google Earth service. Each sub-dataset contains a pair of bitemporal images and the corresponding ground-truth map. The landslide sites in different geographical locations have various sizes, shapes, occurrence times, spatial distributions, phenology states, and land cover types, resulting in considerable spectral heterogeneity and intensity variations in the remote sensing imagery. The GVLM dataset can be used to develop and evaluate machine/deep learning models for change detection, semantic segmentation and landslide extraction. Paper: [Zhang et al., 2023](https://www.sciencedirect.com/science/article/pii/S0924271623000242?dgcid)

- 2023.[**EGY-BCD**](https://github.com/oshholail/EGY-BCD)   
The EGY-BCD dataset is designed to detect building changes from high-resolution satellite imagery with a resolution of 0.25 m/pixel (level 19). The dataset includes four urban and coastal areas in Egypt, collected from Google Earth over two different periods between 2015 and 2022. The dataset contains 6091 pairs of small images of size 256×256 and is randomly divided into three sets: a training set (70%), a validation set (20%), and a test set (10%). The ground-truth data for each pair of images is labeled into two categories, "no-change" or "change," to train the proposed network. Paper: [Holail et al.2023](https://ieeexplore.ieee.org/document/10145434)

- 2023.[**SI-BU dataset**](https://github.com/liaochengcsu/BCE-Net)   
The SI-BU dataset comprises post-phase satellite imagery captured from Google Earth (Google Inc.) in 2021 of Guiyang, Guizhou province, China, along with corresponding labels. The dataset covers an area of approximately 172 km2 and contains buildings of varying height, scale, and appearance. The images and labels were cropped into non-overlapping pairs of 512 × 512 pixels, with 3,604 pairs for training and 1,328 pairs for testing. The labels indicate four categories: background, unchanged buildings, newly constructed buildings, and removed buildings, which are assigned values of 0, 1, 2, and 3, respectively. The labels were meticulously annotated by image interpretation experts to indicate changes between the images and building masks collected from the same location in 2019. The dataset exhibits an off-nadir problem, particularly for high-rise buildings, due to the offset between building rooftops and footprints, which makes it challenging to automatically extract building changes from the dataset. Paper: [Liao et al.2023](https://arxiv.org/abs/2304.07076)

- 2023.[**CNAM-CD**](https://github.com/Silvestezhou/CNAM-CD)   
CNAM-CD is a multi-class change detection dataset that collects images of 12 different urban scenes from the past decade. The dataset selects 12 State-level New Areas in China as the study area and contains 2503 pairs of GeoTiff format images with a pixel size of 512×512. The images were captured at different times from 2013 to 2022. The data source is Google Earth, and the resolution is 0.5m. Paper: [Zhou et al.2023](https://www.mdpi.com/2072-4292/15/9/2464)

- 2023.[**BANDON (Building Change Detection with Off-nadir Aerial Images Dataset)**](https://arxiv.org/abs/2301.10922)   
The BANDON dataset is designed for building change detection using off-nadir aerial images. It consists of 2283 image pairs from urban and rural areas with corresponding change, BT-flows, segmentation, and ST-offsets labels (test sets don't have auxiliary annotations). BANDON provides novel data for the off-nadir building change detection task, and its detailed annotations support multi-task learning in aerial images. Paper: [Pang et al.2023](https://arxiv.org/abs/2301.10922)

- 2022.[**LEVIR Change Captioning (LEVIR-CC) dataset**](https://github.com/Chen-Yang-Liu/RSICC)   
LEVIR-CC dataset contains 10077 pairs of bitemporal RS images and 50385 sentences describing the differences between images. The images of the LEVIR-CC dataset are mainly from the CD dataset LEVIR-CD. LEVIR-CC dataset may help explore models to align visual changes and language in RS images. Paper: [Liu et al.2022](https://ieeexplore.ieee.org/document/9934924)

- 2022.[**DynamicEarthNet**](https://mediatum.ub.tum.de/1650201)   
The DynamicEarthNet dataset includes daily satellite data from January 2018 to December 2019, covering 75 areas of interest around the world with diverse land cover changes. It provides a sequence of daily revisited images for each region, as well as pixel-wise semantic labels for the first day of each month at a resolution of 1024x1024 and pixel granularity of 3 meters, which serve as ground-truth for defining land cover changes over the two-year period. Paper: [Toker A et al.2022](https://arxiv.org/abs/2203.12560)

- 2022.[**Multisource built-up change (MSBC) and multisource OSCD (MSOSCD) datasets**](https://github.com/Lihy256/MSCDUnet)   
The datasets are made to fill the gap of built-up CD datasets including multispectral, SAR, and VHR. MSBC is labeled based on GF-2 VHR images, and the MSOSCD is reformed from an existing dataset—[Onera Satellite CD(OSCD) dataset](https://ieee-dataport.org/open-access/oscd-onera-satellite-change-detection). Paper: [Li et al.2022](https://ieeexplore.ieee.org/document/9791854)

- 2022.[**CLCD dataset**](https://github.com/liumency/CropLand-CD)   
The CLCD dataset consists of 600 pairs image of cropland change samples, with 320 pairs for training, 120 pairs for validation and 120 pairs for testing. The bi-temporal images in CLCD were collected by Gaofen-2 in Guangdong Province, China, in 2017 and 2019, respectively, with spatial resolution ranged from 0.5 to 2 m. Each group of samples is composed of two images of 512 × 512 and a corresponding binary label of cropland change. The main types of change annotated in CLCD include buildings, roads, lakes and bare soil lands, etc. Paper: [Liu et al.2022](https://ieeexplore.ieee.org/document/9780164)

- 2021.[**QFabric**](https://sagarverma.github.io/qfabric)   
QFabric is a comprehensive temporal multi-task dataset with 450,000 change polygons across 504 locations in 100 cities, using imagery from Maxar’s WorldView-2 Satellite collected between January 2014 and July 2020. It includes 6 change types and 9 change status classes, and the accompanying geography and environment metadata provides valuable context for deep neural network development. Paper: [Verma S et al.2021](https://sagarverma.github.io/others/Earthvision_2021_QFabric.pdf)

- 2021.[**HTCD dataset**](https://github.com/ShaoRuizhe/SUNet-change_detection)   
The HTCD dataset, a new Satellite-UAV heterogeneous image data set, was built using the satellite images from [Google Earth](https://www.google.com/earth/) and UAV images from [Open Aerial Map](https://map.openaerialmap.org/). The size of the satellite image is 11 K×15 K pixels. While the UAV image is consisted of 15 image blocks, in total 1.38 M×1.04 M pixels. The ground resolutions of them are 0.5971 m and 7.465 cm, respectively. Images and labels are all stored in GeoTiff format with location information, for the convenience of further analysis and research. Paper: [Shao et al.2021](https://www.mdpi.com/2072-4292/13/18/3750/htm)

- 2021.[**Multi-modal Supervised Change Detection Data**](https://github.com/PatrickTUM/multimodalCD_ISPRS21)   
Sentinel-1 SAR data were provided on the basis of [OSCD dataset](https://ieee-dataport.org/open-access/oscd-onera-satellite-change-detection) for multimodal supervised change detection (SAR-SAR CD or Optical-SAR multi-modal CD). Paper: [Ebel et al.2021](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIII-B3-2021/243/2021/isprs-archives-XLIII-B3-2021-243-2021.pdf)

- 2021.[**S2Looking**](https://github.com/AnonymousForACMMM/Dataset)   
S2Looking, a building change detection dataset that contains large-scale side-looking satellite images captured at varying off-nadir angles. It consists of 5000 registered bitemporal image pairs (size of 1024*1024, 0.5 ~ 0.8 m/pixel) of rural areas throughout the world and more than 65,920 annotated change instances. It provides two label maps to separately indicate the newly built and demolished building regions for each sample in the dataset. Paper: [Shen et al.2021](https://www.mdpi.com/2072-4292/13/24/5094)

- 2021.[**SYSU-CD**](https://github.com/liumency/SYSU-CD)   
The dataset contains 20000 pairs of 0.5-m aerial images of size 256×256 taken between the years 2007 and 2014 in Hong Kong.The main types of changes in the dataset include: (a) newly built urban buildings; (b) suburban dilation; (c) groundwork before construction; (d) change of vegetation; (e) road expansion; (f) sea construction. Paper: [Shi et al.2021](https://ieeexplore.ieee.org/document/9467555)

- 2021.[**Sentinel-2 Multitemporal Cities Pairs (S2MTCP) dataset**](https://zenodo.org/record/4280482#.YBBCX-j7RhE)   
The S2MTCP dataset contains N = 1520 image pairs, spread over all inhabited continents, with the highest concentration of image pairs in North-America, Europe, and Asia. Bands with a spatial resolution smaller than 10 m are resampled to 10 m and images are cropped to approximately 600x600 pixels. It was created for self-supervised training. Paper: [Leenstra et al.2021](https://arxiv.org/abs/2101.08122)

- 2020.[**Hi-UCD**](Hi-UCD)   
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

### Without Label

- [Planet Disaster Datasets](https://www.planet.com/disasterdata/datasets/)   
Planet will make PlanetScope imagery available to the public during a select disaster event.

- [Maxar's Open Data Program](https://www.maxar.com/open-data)   
Maxar will release open imagery (worldview-3 or other) for select sudden onset major crisis events, including pre-event imagery, post-event imagery, and a crowdsourced damage assessment.

- [French National Institute of Geographical and Forest Information (IGN),BD ORTHO](http://professionnels.ign.fr/bdortho)   
The datasets are mosaics of aerial images taken by the French National Institute of Geographical and Forest Information (IGN). They come from a database named BD ORTHO which contains orthorectified aerial images of several regions of France from different years at a resolution of 20 cm or 50 cm per pixel. 

- [LINZ DATA SERVICE](https://data.linz.govt.nz/)   
The New Zealand Land Information Services website provides multi-temporal aerial images of some New Zealand cities, all of which have a resolution of over 1m.

- [USGS EarthExplorer](https://earthexplorer.usgs.gov)   
An epic level database, which can provide multi-temporal，multi-sensor and multi-resolution data.

## Hyperspectral

- 2018.[Hyperspectral Change Detection Dataset](https://citius.usc.es/investigacion/datasets/hyperspectral-change-detection-dataset)   
This dataset can be used to perform change detection techniques in multi-temporal hyperspectral images. It includes two different hyperspectral scenes from the AVIRIS sensor: The Santa Barbara scene, taken on the years 2013 and 2014 with the AVIRIS sensor over the Santa Barbara region (California) whose spatial dimensions are 984 x 740 pixels and includes 224 spectral bands. The Bay Area scene, taken on the years 2013 and 2015 with the AVIRIS sensor surrounding the city of Patterson (California) whose spatial dimensions are 600 x 500 pixels and includes 224 spectral bands.
It also includes a hyperspectral scene from the HYPERION sensor: The Hermiston city scene, taken on the years 2004 and 2007 with the HYPERION sensor over the Hermiston City area (Oregon) whose spatial dimensions are 390 x 200 pixels and includes 242 spectral bands. 5 types of changes related to crop transitions are identified in this scene. Paper: [López-Fandiño et al.2018](https://ieeexplore.ieee.org/document/8518338)

- 2018.[GETNET](https://drive.google.com/file/d/1cWy6KqE0rymSk5-ytqr7wM1yLMKLukfP/view)   
This dataset has two hyperspectral images, which were acquired on May 3, 2013, and December 31, 2013, respectively in Jiangsu province, China. It has a size of 463×241 pixels, with 198 bands available after noisy band removal. In the ground-truth map, white pixels represent changed portions and black pixels mean unchanged parts. Paper: [Wang et al.2018](https://ieeexplore.ieee.org/document/8418840/?denied=)

## 3D

- 2023.[3DCD Dataset](https://sites.google.com/uniroma1.it/3dchangedetection/home-page?pli=1)   
The 3DCD Dataset is designed to facilitate the development of deep learning algorithms that can infer 3D CD maps from remote sensing optical bitemporal images alone, without the need for Digital Elevation Models (DEMs). The dataset comprises pairs of optical images acquired in 2010 and 2017, corresponding 2D and 3D CD maps in raster format (.tiff), and pairs of Digital Surface Models (DSMs) covering the same area and years in the same format (.tiff). Paper: [Marsocci V et al.2023](https://www.sciencedirect.com/science/article/pii/S0924271622003240)

- 2021.[URB3DCD](https://ieee-dataport.org/open-access/urb3dcd-urban-point-clouds-simulated-dataset-3d-change-detection)   
The dataset is based on LoD2 models of [the first and second districts of Lyon](https://geo.data.gouv.fr/datasets/0731989349742867f8e659b4d70b707612bece89), France. To conduct fair qualitative and quantitative evaluation of point clouds change detection techniques. This first version of the dataset is composed of point clouds at a challenging low resolution of around 0.5 points/meter². Paper: [de Gélis et al.2021](https://www.mdpi.com/2072-4292/13/13/2629)

# Code

## Multispectral

### Traditional Method

- [Kondmann L, Toker A, Saha S, et al. SiROC: Spatial Context Awareness for Unsupervised Change Detection in Optical Satellite Images](https://github.com/lukaskondmann/SiROC). TGRS 2021

- [Lv Z, Wang F J, Liu T, et al. Novel Automatic Approach for Land Cover Change Detection by Using VHR Remote Sensing Images](https://github.com/TongfeiLiu/ASEA-CD). GRSL 2021

- 2019.[Bobholamovic/ChangeDetectionToolbox](https://github.com/Bobholamovic/ChangeDetectionToolbox)

- 2019.[Canty M J. Image Analysis, Classification and Change Detection in Remote Sensing (Fourth Revised Edition)](https://github.com/mortcanty/CRC4Docker)

- 2017.[Canty M J. Change Detection with Google Earth Engine Imagery](https://github.com/mortcanty/earthengine)

- 2014.[Canty M J. Image Analysis, Classification and Change Detection in Remote Sensing (Third Revised Edition)](https://github.com/mortcanty/CRCPython)

- [Zhu Z, Woodcock C E, et al. Algorithm developed for Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data](https://github.com/GERSL/CCDC)

- [Li X, Liu X, Liang X, et al. Geographical Simulation and Optimization System (GeoSOS)](https://www.geosimulation.cn/index.html)

- Implementation of " [2009.Celik T. Unsupervised change detection in satellite images using principal component analysis and k-means clustering](https://ieeexplore.ieee.org/abstract/document/5196726/) ".  
[Matlab](https://github.com/rulixiang/ChangeDetectionPCAKmeans), [Python](https://github.com/abhijeet3922/Change-Detection-in-Satellite-Imagery)

- [Nielsen A A.The Regularized Iteratively Reweighted Multivariate Alteration Detection (IR-MAD)](http://people.compute.dtu.dk/alan/software.html). TIP 2007

### Deep Learning

#### 2D

- [Ding L, Zhu K, Peng D, et al. Adapting Segment Anything Model for Change Detection in HR Remote Sensing Images](https://github.com/ggsDing/SAM-CD). arXiv 2023

- [Zheng Z, Tian S, Ma A, et al. Scalable Multi-Temporal Remote Sensing Change Data Generation via Simulating Stochastic Change Process](https://github.com/Z-Zheng/Changen). ICCV 2023

- [Bernhard M, Strauß N, Schubert M. MapFormer: Boosting Change Detection by Using Pre-change Information](https://github.com/mxbh/mapformer). ICCV 2023 

- [Mall U, Hariharan B, Bala K. Change-Aware Sampling and Contrastive Learning for Satellite Images](https://github.com/utkarshmall13/caco). CVPR 2023

- [Xing Y, Jiang J, Xiang J, et al. LightCDNet: Lightweight Change Detection Network Based on VHR Images](https://github.com/NightSongs/LightCDNet). GRSL 2023

- [Lei T, Geng X, Ning H, et al. Ultralightweight Spatial–Spectral Feature Cooperation Network for Change Detection in Remote Sensing Images](https://github.com/SUST-reynole/USSFC-Net). TGRS 2023

- [Li Z, Tang C, Liu X, et al. Lightweight Remote Sensing Change Detection with Progressive Feature Aggregation and Supervised Attention](https://github.com/guanyuezhen/A2Net). TGRS 2023

- [Feng Y, Jiang J, Xu H, et al. Change Detection on Remote Sensing Images using Dual-branch Multi-level Inter-temporal Network](https://github.com/ZhengJianwei2/DMINet). TGRS 2023

- [Seo M, Lee H, Jeon Y, et al. Self-Pair: Synthesizing Changes from Single Source for Object Change Detection in Remote Sensing Imagery](https://github.com/seominseok0429/Self-Pair-for-Change-Detection). WACV2023

- [Fang S, Li K, Li Z. Changer: Feature Interaction is What You Need for Change Detection](https://github.com/likyoo/open-cd/tree/main/configs/changer). TGRS 2023

- [Chen H, Pu F, Yang R, et al. RDP-Net: Region detail preserving network for change detection](https://github.com/Chnja/RDPNet). TGRS 2022

- [Cao Y, Huang X. A full-level fused cross-task transfer learning method for building change detection using noise-robust pretrained networks on crowdsourced labels](https://github.com/lauraset/FFCTL). RSE 2022

- [Chen H, Li W, Chen S, et al. Semantic-aware Dense Representation Learning for Remote Sensing Image Change Detection](https://github.com/justchenhao/SaDL_CD). TGRS 2022

- [Codegoni A, Lombardi G, Ferrari A. TINYCD: A (Not So) Deep Learning Model For Change Detection](https://github.com/AndreaCodegoni/Tiny_model_4_CD).  Neural Computing and Applications 2022

- [Pei G, Zhang L. Feature Hierarchical Differentiation for Remote Sensing Image Change Detection](https://github.com/ZSVOS/FHD). GRSL 2022

- 2022.[likyoo/Open-CD](https://github.com/likyoo/open-cd): Open-CD is an open source change detection toolbox based on a series of open source general vision task tools.

- [Shi N, Chen K, Zhou G. A Divided Spatial and Temporal Context Network for Remote Sensing Change Detection](https://github.com/shinianzhihou/ChangeDetection#). JSTARS 2022

- [Liu M, Chai Z, Deng H, et al. A CNN-transformer Network with Multi-scale Context Aggregation for Fine-grained Cropland Change Detection](https://github.com/liumency/CropLand-CD). JSTARS 2022

- [Liu J, Xuan W, Gan Y, et al. An End-to-end Supervised Domain Adaptation Framework for Cross-Domain Change Detection](https://github.com/Perfect-You/SDACD). Pattern Recognition 2022   

- 2022.[PaddleRS](https://github.com/PaddlePaddle/PaddleRS): Awesome Remote Sensing Toolkit based on PaddlePaddle

- [Ding L, Guo H, Liu S, et al. Bi-temporal semantic reasoning for the semantic change detection in HR remote sensing images](https://github.com/ggsDing/Bi-SRNet). TGRS 2022

- [Bandara W G C, Nair N G, Patel V M. DDPM-CD: Remote Sensing Change Detection using Denoising Diffusion Probabilistic Models](https://github.com/wgcban/ddpm-cd). arXiv 2022

- [Bandara W G C, Patel V M. Revisiting Consistency Regularization for Semi-supervised Change Detection in Remote Sensing Images](https://github.com/wgcban/SemiCD). arXiv 2022

- [Bandara W G C, Patel V M. A Transformer-Based Siamese Network for Change Detection](https://github.com/wgcban/ChangeFormer). IGARSS 2022

- [Saha S, Ebel P, Zhu X X. Self-supervised multisensor change detection](https://gitlab.lrz.de/ai4eo/cd/-/tree/main/sarOpticalMultisensorTgrs2021). TGRS 2022

- [Chen P, Hong D, Chen Z, et al. FCCDN: Feature Constraint Network for VHR Image Change Detection](https://github.com/chenpan0615/FCCDN_pytorch). ISPRS P&RS 2022

- 2021.[Bobholamovic/CDLab](https://github.com/Bobholamovic/CDLab): Yet another repository for developing and benchmarking deep learning-based change detection methods

- 2021.[shinianzhihou/ChangeDetection](https://github.com/shinianzhihou/ChangeDetection): A framework for change detection using PyTorch

- [Shi Q, Liu M, Li S, et al. A Deeply Supervised Attention Metric-Based Network and an Open Aerial Image Dataset for Remote Sensing Change Detection](https://github.com/liumency/DSAMNet). TGRS 2021

- [Shao R, Du C, Chen H, et al. SUNet: Change Detection for Heterogeneous Remote Sensing Images from Satellite and UAV Using a Dual-Channel Fully Convolution Network](https://github.com/ShaoRuizhe/SUNet-change_detection). Remote Sensing 2021

- [Diakogiannis F I, Waldner F, Caccetta P. Looking for change? Roll the Dice and demand Attention](https://github.com/feevos/ceecnet). Remote Sensing 2021

- [Papadomanolaki M, Vakalopoulou M, Karantzalos K. A Deep Multi-Task Learning Framework Coupling Semantic Segmentation and Fully Convolutional LSTM Networks for Urban Change Detection](https://github.com/mpapadomanolaki/multi-task-L-UNet). TGRS 2021

- [Zheng Z, Zhong Y, Wang J, et al. Building damage assessment for rapid disaster response with a deep object-based semantic change detection framework: from natural disasters to man-made disasters](https://github.com/Z-Zheng/ChangeOS). RSE 2021

- [Xu J, Luo C, Chen X, et al. Remote Sensing Change Detection Based on Multidirectional Adaptive Feature Fusion and Perceptual Similarity](https://github.com/wzjialang/MFPNet). Remote Sensing 2021

- [Zhang H, Lin M, Yang G, et al. ESCNet: An End-to-End Superpixel-Enhanced Change Detection Network for Very-High-Resolution Remote Sensing Images](https://github.com/Bobholamovic/ESCNet). TNNLS 2021

- [Mañas O, Lacoste A, Giro-i-Nieto X, et al. Seasonal Contrast: Unsupervised Pre-Training from Uncurated Remote Sensing Data](https://github.com/ElementAI/seasonal-contrast). ICCV 2021

- [Zheng Z, Ma A, Zhang L, et al. Change is Everywhere: Single-Temporal Supervised Object Change Detection for High Spatial Resolution Remote Sensing Imagery](https://github.com/Z-Zheng/ChangeStar). ICCV 2021

- [Liu M, Shi Q, Marinoni A, et al. Super-resolution-based Change Detection Network with Stacked Attention Module for Images with Different Resolutions](https://github.com/liumency/SRCDNet). TGRS 2021

- [Chen H, Qi Z, Shi Z. Remote Sensing Image Change Detection with Transformers](https://github.com/justchenhao/BIT_CD).TGRS 2021   

- [Chen H, Li W, Shi Z. Adversarial Instance Augmentation for Building Change Detection in Remote Sensing Images](https://github.com/justchenhao/IAug_CDNet).TGRS 2021 

- [Fang S, Li K, Shao J, et al. SNUNet-CD: A Densely Connected Siamese Network for Change Detection of VHR Images](https://github.com/likyoo/Siam-NestedUNet). GRSL 2021 

- 2020.[ChenHongruixuan/ChangeDetectionRepository](https://github.com/ChenHongruixuan/ChangeDetectionRepository)

- 2020.[llu025/Heterogeneous_CD](https://github.com/llu025/Heterogeneous_CD)

- [Daudt R C, Le Saux B, Boulch A. Fully convolutional siamese networks for change detection](https://github.com/rcdaudt/fully_convolutional_change_detection). ICIP 2018

#### 3D
- [Marsocci V, Coletta V, Ravanelli R, et al. Inferring 3D change detection from bitemporal optical images](https://github.com/VMarsocci/3DCD). ISPRS P&RS 2023
- 2023.[de Gélis I, Lefèvre S, Corpetti T. Siamese KPConv: 3D multiple change detection from raw point clouds using deep learning](https://github.com/IdeGelis/torch-points3d-SiameseKPConv). ISPRS P&RS 2023

## SAR
- [Alatalo J, Sipola T, Rantonen M. Improved Difference Images for Change Detection Classifiers in SAR Imagery Using Deep Learning](https://github.com/janne-alatalo/sar-change-detection). TGRS 2023
- [Qu X, Gao F, Dong J, et al. Change Detection in Synthetic Aperture Radar Images Using a Dual-Domain Network](https://github.com/summitgao/SAR_CD_DDNet). GRSL 2022

## Hyperspectral
- [Wang Y, Hong D, Sha J, et al. Spectral–spatial–temporal transformers for hyperspectral image change detection](https://github.com/yanhengwang-heu/IEEE_TGRS_SSTFormer). TGRS 2022
- [Hu M, Wu C, Zhang L, et al. Hyperspectral anomaly change detection based on autoencoder](https://github.com/meiqihu/ACDA). JSTARS 2021


# Contest   

**Please note that some of the datasets in these competitions are publicly available, such as xView2 and SpaceNet7.**

- [**2023 “吉林一号”杯卫星遥感应用青年创新创业大赛-基于高分辨率卫星影像的耕地变化检测**](https://www.jl1mall.com/contest/match/info?id=1645664411716952066) *(长光卫星, 2023年5月)*   
耕地变化检测存在变化类型多、变化目标小的检测难点，因此需要研发一种基于高分辨率遥感影像的耕地变化检测算法，提高耕地变化检测中小目标的召回率和耕地变化类型的分类准确率，推动算法在“非农化”、耕地保护等实际需求中的应用。数据: 吉林一号，分辨率优于0.75米。类别描述：耕地变为道路，耕地变为林草，耕地变为建筑，耕地变为其他，道路变为耕地，林草变为耕地，建筑变为耕地，其他变为耕地，非“耕地变化”变化区域。图像尺寸：256×256像素。初赛数据量：共计8000余组，训练集6000余组,每组包含2个时相影像及标签；测试集2000余组,每组包含2个时相影像。

- [**2022 The SpaceNet 8 Flood Detection Challenge**](https://medium.com/@SpaceNet_Project/the-spacenet-8-flood-detection-challenge-dataset-and-algorithmic-baseline-release-e0c9f5a44154) *(SpaceNet, Maxar, Jul 2022)*   
Three areas of interest (AOIs) were selected for the dataset consisting of 12 Maxar satellite images of both pre- and post-flooding event imagery. Along with the imagery, hand labeled building footprints, road and flood attributes are provided for training and scoring. The AOIs include Germany with flooding from heavy rains in July 2021, Louisiana following Hurricane Ida in August 2021, and a “mystery” location that will be used to test the top 10 algorithms from the public leaderboard for final scoring after the challenge has concluded. Baseline: [SpaceNetChallenge/SpaceNet8](https://github.com/SpaceNetChallenge/SpaceNet8). Paper: [Hänsch, Ronny, et al.2022](https://openaccess.thecvf.com/content/CVPR2022W/EarthVision/papers/Hansch_SpaceNet_8_-_The_Detection_of_Flooded_Roads_and_Buildings_CVPRW_2022_paper.pdf).

- **2021 “昇腾杯”遥感影像智能处理算法大赛-耕地建筑物变化检测** *(武汉大学, 2021年9月)*   
通过前后两时相的遥感影像，提取出地物发生变化的像元并赋予变化标签。 依据所述地物变化标准，以耕地-建筑/动土的像素级变化检测为目标。数据为1-2米分辨率光学遥感影像，6000+张遥感影像变化检测样本数据(按512 X 512大小折算)。标签格式为单通道的png，每个像素的标签值由一个数值表示， 使用‘uint8’数据类型存储，该数值表示是否为变化，“0”代表未变化，“1”代表变化。Top4解决方案详见[WangZhenqing-RS/2021rsipac_changeDetection_TOP4](https://github.com/WangZhenqing-RS/2021rsipac_changeDetection_TOP4)，Top5解决方案详见[78666621/2021rsipac_changeDetection_TOP5](https://github.com/78666621/2021rsipac_changeDetection_TOP5)  

- [**2021 遥感图像智能解译技术挑战赛-建筑物变化检测**](https://captain-whu.github.io/PRCV2021_RS/index.html) *(武汉大学, 航天宏图. 2021年8月)*   
本竞赛数据集主要包含涉及建筑物的地物变化。全部图像数据共10000对（训练集：6000对图像，验证集：2000对图像，测试样本：2000对图像），尺寸为512 x 512，主要分布于北京、上海、广州以及杭州等城市。部分数据源自[SECOND](http://www.captain-whu.com/PROJECT/SCD/)数据集。第二名解决方案详见[businiaoo/PRCV2021-Change-Detection-Contest-2nd-place-Solution](https://github.com/businiaoo/PRCV2021-Change-Detection-Contest-2nd-place-Solution), 第三名解决方案详见[likyoo/PRCV2021_ChangeDetection_Top3](https://github.com/likyoo/PRCV2021_ChangeDetection_Top3)。

- [**2021 第五届“中科星图杯”国际高分遥感图像解译大赛-高分辨率可见光图像中建筑物普查与变化检测**](http://gaofen-challenge.com/challenge) *(中国科学院空天信息创新研究院. 2021年8月)*    
高分二号、吉林一号光学数据，分辨率优于1m。每幅图像对建筑物进行像素级标注，同一时相数据对变化的建筑物区域进行像素级标注。建筑物提取类别：建筑物和背景，变化检测类别：变化的建筑区域和非变化的建筑区域。

- [**2021 慧眼“天智杯”人工智能挑战赛-可见光建筑智能变化检测**](https://www.rsaicp.com/portal/contestDetail?id=1&tab=rule) *(北京市遥感信息研究所，中国科学院人工智能创新研究院. 2021年6月)*    
每组数据包含前时相遥感图像，后时相遥感图像以及对应的建筑变化标签图。影像格式为png，包含R、G、B三个波段，影像尺寸为1024 X 1024像素，分辨率为0.5~0.7米。标签图与图像等大，其中 (0,0,0) 代表没有建筑变化，(0,0,255) 代表建筑增加，(255,0,0) 代表建筑减少。

- [**2021 DynamicEarthNet Challenge**](http://www.classic.grss-ieee.org/earthvision2021/challenge.html) *(TUM, DLR, panet. Mar 2021)*    
The challenge consists of two tracks (**Unsupervised Binary Land Cover Change Detection** and **Weakly-Supervised Multi-Class Change Detection**) in which participants are tasked to detect multi-temporal changes with few or no training labels. The first solution can be found [solcummings/earthvision2021-weakly-supervised](https://github.com/solcummings/earthvision2021-weakly-supervised).

- [**2021 IEEE GRSS Data Fusion Contest: Track MSD (Multitemporal Semantic Change Detection)**](https://www.grss-ieee.org/community/technical-committees/2021-ieee-grss-data-fusion-contest-track-msd/) *(GRSS, Microsoft. Jan 2021)*   
The task of Track MSD is to create bitemporal high resolution land cover maps using only low-resolution and noisy land cover labels for training. Such a scenario is often encountered around the world, as the proliferation of new sensors with either high spatial resolution (submeter) or high temporal resolution (weekly or even daily) remains unmatched by equally rich label data. Instead, detecting change would have to rely on the analysis of a sequence of input images in an unsupervised manner or with aid of weak, noisy, and outdated labels. Paper: [Li Z et al. 2022](https://ieeexplore.ieee.org/document/9690575).

- [**2020 SpaceNet 7: Multi-Temporal Urban Development Challenge**](https://medium.com/the-downlinq/the-spacenet-7-multi-temporal-urban-development-challenge-dataset-release-9e6e5f65c8d5) *(CosmiQ Works, Planet. Aug 2020)*   
In this challenge, participants will identify and track buildings in satellite imagery time series collected over rapidly urbanizing areas. The competition centers around a new open source dataset of Planet satellite imagery mosaics, which will include 24 images (one per month) covering ~100 unique geographies. The dataset will comprise 40,000 km2 of imagery and exhaustive polygon labels of building footprints in the imagery, totaling over 3M individual annotations. Challenge participants will be asked to track building construction over time, thereby directly assessing urbanization. For details about the solution, see [SpaceNetChallenge/SpaceNet7_Multi-Temporal_Solutions](https://github.com/SpaceNetChallenge/SpaceNet7_Multi-Temporal_Solutions).

- [**2020 商汤科技首届AI遥感解译大赛-变化检测赛道**](https://rs.sensetime.com/competition/index.html#/info) *(商汤. 2020年8月)*   
数据集：4662组，分辨率：0.5~3m，规格：512*512，变化类型为6种主要土地性质之间的相互转化：水体、地面、低矮植被、树木、建筑物、运动场。每组数据中，前后时相的两张图片各自对应一张标注图，表示发生变化的区域以及该图片变化区域内各时期的土地性质。第一名的解决方案详见 [LiheYoung/SenseEarth2020-ChangeDetection](https://github.com/LiheYoung/SenseEarth2020-ChangeDetection)。

- [**2019 xView 2 Building Damage Asessment Challenge**](https://xview2.org) *(DIUx, Nov 2019)*     
550k building footprints & 4 damage scale categories, 20 global locations and 7 disaster types (wildfire, landslides, dam collapses, volcanic eruptions, earthquakes/tsunamis, wind, flooding), Worldview-3 imagery (0.3m res.), pre-trained baseline model. Paper: [Gupta et al. 2019](https://arxiv.org/abs/1911.09296)

- [**2019 遥感图像稀疏表征与智能分析竞赛-变化检测赛道**](http://rscup.bjxintong.com.cn/#/theme/4) *(武汉大学. 2019年7月)*   
本项竞赛以光学遥感图像为处理对象，参赛队伍使用主办方提供的遥感图像进行建筑物变化检测，主办方根据评分标准对变化检测结果进行综合评价。竞赛中将提供两个不同时间获取的大尺度高分辨率遥感图像（包含蓝、绿、红和近红外四个波段），以及图像中变化区域的二值化标注数据集。

- [**2017 广东政务数据创新大赛—智能算法赛**](https://tianchi.aliyun.com/competition/entrance/231615/introduction) *(阿里巴巴. 2017年11月)*    
使用2015年和2017年分别获取到的广东省某地的Quickbird卫星影像（包含蓝、绿、红和近红外四个波段），识别出两年之间新增的人工地上建筑物（不包括道路）。获胜团队的解决方案可以在[天池](https://tianchi.aliyun.com/forum/postDetail?postId=3527)官网上找到。

# Reference

- [chrieke/awesome-satellite-imagery-datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [MinZHANG-WHU/Change-Detection-Review](https://github.com/MinZHANG-WHU/Change-Detection-Review)
