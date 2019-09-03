# Awesome Remote Sensing Change Detection [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

List of datasets, codes, researchers and contests related to remote sensing change detection.The newest at the top of each category.

![](/2018.recurrent&#32;convolutional&#32;neural&#32;network.jpg)



## 1. Dateset

### 1.1 Multispectral 

- 2019.[Detecting Urban Changes with Recurrent Neural Networks from Multitemporal Sentinel-2 Data](https://github.com/granularai/ChangeDetection)
  
- 2019.[Wuhan multi-temperature scene (MtS-WH) Dataset](http://sigma.whu.edu.cn/newspage.php?q=2019_03_26)   
The dataset is mainly used for theoretical research and verification of **scene change detection** methods. It consists of two large-size **VHR** images, which have a size of 7200x6000 and are respectively acquired by **IKONOS** sensors in Feb, 2002 and Jun, 2009. The images cover the Hanyang District, Wuhan City, China and contain 4 spectral bands (Blue, Green, Red and Near-Infrared). The spatial resolution of the images is 1m after fusion of the pan and multispectral images by the Gram–Schmidt algorithm.

- 2018.[Onera Satellite Change Detection Dataset](https://rcdaudt.github.io/oscd/)   
This dataset addresses the issue of detecting changes between satellite images from different dates. It comprises 24 pairs of **multispectral** images taken from the **Sentinel-2** satellites between 2015 and 2018. Locations are picked all over the world, in Brazil, USA, Europe, Middle-East and Asia. For each location, registered pairs of 13-band multispectral satellite images obtained by the Sentinel-2 satellites are provided. Images vary in spatial resolution between 10m, 20m and 60m.

- 2017.[Damage Detection from Aerial Images via Convolutional Neural Networks(ABCDdataset)](https://github.com/gistairc/ABCDdataset)   
This is a new labeled dataset, specially geared toward constructing and evaluating damage detection systems to identify whether buildings have been washed-away by tsunami.These pairs were cropped from a hefty number of RGB **aerial** images of Tohoku region of Japan. These aerial images were taken before or after the Great East Japan earthquake, with the original pixel resolution of 40 cm for pre-quake images and 12 cm for post-qukae images (actually, resampled to 40 cm).

- 2015.[Spectral alignment of multi-temporal cross-sensor images with automated kernel canonical correlation analysis](https://sites.google.com/site/michelevolpiresearch/codes/cross-sensor) 

- 2008.[SZTAKI AirChange Benchmark set](http://web.eee.sztaki.hu/remotesensing/airchange_benchmark.html)   
This Benchmark set contains 13 **aerial** image pairs of size 952x640 and resolution **1.5m**/pixel and binary change masks (drawn by hand).Each record constains a pair of preliminary registered input images and a mask of the 'relevant' changes. The input images are taken with 5, 7 resp. 23 years time differences. During the generation of the change mask, we have considered the following differences as relevant changes: (a) new built-up regions (b) building operations (c) planting of large group of trees (d) fresh plough-land (e) groundwork before building over. Note that the ground truth does NOT contain change classification, only binary change-no change decision for each pixel.   
**Note**: This maybe the most frequently used dataset in the paper of remote sensing change detection.

- [WUDA-RS-Img(wuhan university datasets of annotated remote sensing images)](http://captain.whu.edu.cn/WUDA-RSImg/index.html)   
The dataset about change detection will be released in the future  (perhaps never will, waiting too long).

- [DigitalGlobe's Open Data Program](https://www.digitalglobe.com/opendata/all-events)   
 DigitalGlobe will release open imagery (worldview-3 or other) for select sudden onset major crisis events, including pre-event imagery, post-event imagery and a crowdsourced damage assessment.

- [French National Institute of Geographical and Forest Information (IGN),bdortho](http://professionnels.ign.fr/bdortho)  

- [LINZ DATA SERVICE](https://data.linz.govt.nz/)
    - [AIRS (Aerial Imagery for Roof Segmentation)](https://www.airs-dataset.com/)



### 1.2 Hyperspectral 

- 2018.[Stacked autoencoders for multiclass change detection in hyperspectral images](https://citius.usc.es/investigacion/datasets/hyperspectral-change-detection-dataset)

- 2018.[GETNET: A General End-to-End 2-D CNN Framework for Hyperspectral Image Change Detection](https://drive.google.com/file/d/1cWy6KqE0rymSk5-ytqr7wM1yLMKLukfP/view)


### 1.3 CV

- 2014.[CDnet (video change detection)](http://changedetection.net/)

- 2015.[Change Detection from a Street Image Pair using CNN Features and Superpixel Segmentation](http://www.vision.is.tohoku.ac.jp/us/research/4d_city_modeling/pano_cd_dataset/)

- 2018.[Fully Convolutional Siamese Network for Scene Change Detection](https://github.com/gmayday1997/SceneChangeDet)



## 2. Code

## 2.1. Multispectral

### 2.1.1 Traditional Method 

- 2019.[M J Canty. Image Analysis, Classification and Change Detection in Remote Sensing(Fourth Revised Edition)](https://github.com/mortcanty/CRC4Docker)

- 2017.[M J Canty. Change Detection with Google Earth Engine Imagery](https://github.com/mortcanty/earthengine)

- 2014.[M J Canty. Image Analysis, Classification and Change Detection in Remote Sensing(Third Revised Edition)](https://github.com/mortcanty/CRCPython)

- [Zhu Zhe.Algorithm developed for Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data](https://github.com/GERSL/CCDC)

- Implementation of " [2009.Celik T. Unsupervised change detection in satellite images using principal component analysis and k-means clustering](https://ieeexplore.ieee.org/abstract/document/5196726/) ".  
[Matlab](https://github.com/rulixiang/ChangeDetectionPCAKmeans),[Python](https://github.com/abhijeet3922/Change-Detection-in-Satellite-Imagery)

- 2007.[IR-MAD(The Regularized Iteratively Reweighted Multivariate Alteration Detection)](http://people.compute.dtu.dk/alan/software.html)

### 2.1.2 Deep Learning

- [Rodrigo Caye Daudt](https://rcdaudt.github.io/)
  - 2019.[Guided anisotropic diffusion (GAD) ](https://github.com/rcdaudt/guided_anisotropic_diffusion)
  - 2018.[ Fully convolutional change detection](https://github.com/rcdaudt/fully_convolutional_change_detection)
  - 2018.[Patch based change detection](https://github.com/rcdaudt/patch_based_change_detection)

- 2019.[Maria Papadomanolaki,et al. Detecting Urban Changes with Recurrent Neural Networks from Multitemporal Sentinel-2 Data (IGARSS 2019)](https://github.com/granularai/ChangeDetection)

- 2019.[DSFANet (Deep Slow Feature Analysis Network)](https://github.com/rulixiang/DSFANet)

- 2019.[End-to-End Change Detection for High Resolution Satellite Images Using Improved UNet++](https://github.com/daifeng2016/End-to-end-CD-for-VHR-satellite-image)

- 2018.[Rahman F, Vasu B, Van Cor J, et al. Siamese Network with Multi-level Features for Patch-based Change Detection in Satellite Imagery](https://github.com/vbhavank/Siamese-neural-network-for-change-detection)

- 2018.[Enqiang Guo, Xinsha Fu,et al.Learning to Measure Changes: Fully Convolutional Siamese Metric Networks for Scene Change Detection](https://github.com/gmayday1997/SceneChangeDet)

- 2018.[Shishira R Maiya,et al.Slum Segmentation and Change Detection : A Deep Learning Approach](https://github.com/cbsudux/Mumbai-slum-segmentation)

- 2016.[El Amin A M, Liu Q, Wang Y. Convolutional neural network features based change detection in satellite images](https://github.com/vbhavank/Unstructured-change-detection-using-CNN)



## 2.2 SAR
- [Feng Gao](https://summitgao.github.io/)
  - 2019.[Sea ice change detection in SAR images based on convolutional-wavelet neural networks(Matlab)](https://github.com/summitgao/SAR_Change_Detection_CWNN)
  - 2019.[Transferred deep learning for sea ice change detection from synthetic aperture radar images(Matlab)](https://github.com/summitgao/SAR-Change-Detection-MLFN)

- 2015.[Knut Conradsen,et al.Change detection in polarimetric SAR images in Python](https://github.com/fouronnes/SAR-change-detection)



## 3. Researcher

### 3.1 Team

**University of Trento**
- [RSLAB(Remote Sensing Laboratory)](https://rslab.disi.unitn.it/people/) - Lorenzo Bruzzone 
  
**Wuhan University**
- [CVEO(Computer Vision for Earth Observation team)](https://cveo.github.io/) - Xiaodong Zhang 
- [Sigma(Sensing Intelligence, Geoscience and MAchine learning lab)](http://sigma.whu.edu.cn/index.php) - Bo Du
- [CAPTAIN(Computational and Photogrammetric Vision Team)](http://captain.whu.edu.cn/index.html) - Gui-Song Xia


**Xidian University**
- [OMEGA(Optimization and Mining Knowledge via Artificial Intelligence)](http://web.xidian.edu.cn/mggong/index.html) - Maoguo Gong

**University of Connecticut**
- [GERS Lab(Global Environmental Remote Sensing Laboratory)](https://gerslab.uconn.edu/) - Zhe Zhu



## 4.Contest

- [**xView 2 Building Damage Asessment Challenge**](https://xview2.org) *(DIUx, Nov 2019)*  
550k building footprints & 4 damage scale categories, 20 global locations and 7 disaster types (wildfire, landslides, dam collapses, volcanic eruptions, earthquakes/tsunamis, wind, flooding), Worldview-3 imagery (0.3m res.), pre-trained baseline model. Paper: [Gupta et al. 2019](http://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_Creating_xBD_A_Dataset_for_Assessing_Building_Damage_from_Satellite_CVPRW_2019_paper.html)

- [**遥感图像稀疏表征与智能分析竞赛-变化检测**](http://rscup.bjxintong.com.cn/#/theme/4) *(Wuhan University et al.Jul 2019)*     
本项竞赛以光学遥感图像为处理对象，参赛队伍使用主办方提供的遥感图像进行建筑物变化检测，主办方根据评分标准对变化检测结果进行综合评价。竞赛中将提供两个不同时间获取的大尺度高分辨率遥感图像（包含蓝、绿、红和近红外四个波段），以及图像中变化区域的二值化标注数据集。   

- [**广东政务数据创新大赛—智能算法赛**](https://tianchi.aliyun.com/competition/entrance/231615/introduction) *(Alibaba et al.Nov 2017)*    
  使用2015年和2017年分别获取到的广东省某地的Quickbird卫星影像（包含蓝、绿、红和近红外四个波段），识别出两年之间新增的人工地上建筑物（不包括道路）。获胜团队的解决方案可以在[天池](https://tianchi.aliyun.com/forum/postDetail?postId=3527)官网上找到。
  


## Reference
- [Awesome Satellite Imagery Datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [Zhang Bin's Blog. remote sensing datasets](https://zhangbin0917.github.io/2018/06/12/%E9%81%A5%E6%84%9F%E6%95%B0%E6%8D%AE%E9%9B%86/)
- The picture of this page is from [Mou L et al.2019](https://ieeexplore.ieee.org/document/8541102)
  


