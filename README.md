# Awesome Remote Sensing Change Detection [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

List of datasets, codes, papers, and contests related to remote sensing change detection.

![](/2018.recurrent&#32;convolutional&#32;neural&#32;network.jpg)



## 1 Dateset

### 1.1 Multispectral 

#### With label

- 2019.[Wuhan multi-temperature scene (MtS-WH) Dataset](http://sigma.whu.edu.cn/newspage.php?q=2019_03_26)   
The dataset is mainly used for theoretical research and verification of **scene change detection** methods. It consists of two large-size **VHR** images, which have a size of 7200x6000 and are respectively acquired by **IKONOS** sensors in Feb 2002 and Jun 2009. The images cover the Hanyang District, Wuhan City, China and contain 4 spectral bands (Blue, Green, Red, and Near-Infrared). The spatial resolution of the images is 1m after fusion of the pan and multispectral images by the Gram–Schmidt algorithm.

- 2018.[Lebedev M A, Vizilter Y V, Vygolov O V, et al. Change detection in remote sensing images using conditional adversarial networks](https://drive.google.com/file/d/1GX656JqqOyBi_Ef0w65kDGVto-nHrNs9/edit)   
This dataset has three types: synthetic images without objects relative shift, synthetic images with small relative shift of objects, real season-varying remote sensing images(obtained by **Google Earth**). The real season-varying remote sensing images have 16000 image sets with image size 256x256 pixels(10000 train sets and 3000 test and validation sets) and a spatial resolution of **3 to 100 cm/px**.

- 2018.[Onera Satellite Change Detection Dataset](https://rcdaudt.github.io/oscd/)   
This dataset addresses the issue of detecting changes between satellite images from different dates. It comprises 24 pairs of **multispectral** images taken from the **Sentinel-2** satellites between 2015 and 2018. Locations are picked all over the world, in Brazil, USA, Europe, Middle-East and Asia. For each location, registered pairs of 13-band multispectral satellite images obtained by the Sentinel-2 satellites are provided. Images vary in spatial resolution between 10m, 20m, and 60m.

- 2011.[The Aerial Imagery Change Detection (AICD) dataset](https://computervisiononline.com/dataset/1105138664)   
This dataset contains **synthetic aerial images** with artificial changes generated with a rendering engine. It contains 1000 pairs of 800x600 images, each pair consisting of one reference image and one test image, and the 1000 corresponding 800x600 ground truth masks. 

- 2008.[SZTAKI AirChange Benchmark set](http://web.eee.sztaki.hu/remotesensing/airchange_benchmark.html)   
This dataset contains 13 **aerial** image pairs of size 952x640 and resolution **1.5m/pixel** and binary change masks (drawn by hand). Each record contains a pair of preliminary registered input images and a mask of the 'relevant' changes. The input images are taken with 5, 7 resp. 23 years of time differences. During the generation of the change mask, we have considered the following differences as relevant changes: (a) new built-up regions (b) building operations (c) planting of large group of trees (d) fresh plow-land (e) groundwork before building over. Note that the ground truth does NOT contain change classification, only binary change-no change decision for each pixel.   
**Note**: This may be the most frequently used dataset in the paper.


#### Without label
- [WUDA-RS-Img (Wuhan University Datasets of Annotated Remote Sensing Images)](http://captain.whu.edu.cn/WUDA-RSImg/index.html)   
The dataset about change detection will be released in the future.

- [Planet Disaster Datasets](https://www.planet.com/disasterdata/datasets/)   
Planet will make PlanetScope imagery available to the public during a select disaster event. 

- [DigitalGlobe's Open Data Program](https://www.digitalglobe.com/opendata/all-events)   
 DigitalGlobe will release open imagery (**worldview-3** or other) for select sudden onset major crisis events, including pre-event imagery, post-event imagery, and a crowdsourced damage assessment.

- [French National Institute of Geographical and Forest Information (IGN),BD ORTHO](http://professionnels.ign.fr/bdortho)   
The datasets are mosaics of **aerial** images taken by the French National Institute of Geographical and Forest Information (IGN). They come from a database named BD ORTHO which contains orthorectified aerial images of several regions of France from different years at a resolution of **20 cm** or **50 cm** per pixel. 

- [LINZ DATA SERVICE](https://data.linz.govt.nz/)   
The New Zealand Land Information Services website provides multi-temporal **aerial** images of some New Zealand cities, all of which have a resolution of **over 1m**.

- [USGS EarthExplorer](https://earthexplorer.usgs.gov)   
An epic level database, which can provide multi-temporal，multi-sensor and multi-resolution data. 


### 1.2 Hyperspectral 

- 2018.[Hyperspectral Change Detection Dataset](https://citius.usc.es/investigacion/datasets/hyperspectral-change-detection-dataset)   
This dataset can be used to perform change detection techniques in multi-temporal hyperspectral images. 
It includes two different hyperspectral scenes from the **AVIRIS** sensor: The Santa Barbara scene, taken on the years 2013 and 2014 with the AVIRIS sensor over the Santa Barbara region (California) whose spatial dimensions are 984 x 740 pixels and includes 224 spectral bands. The Bay Area scene, taken on the years 2013 and 2015 with the AVIRIS sensor surrounding the city of Patterson (California) whose spatial dimensions are 600 x 500 pixels and includes 224 spectral bands.
It also includes a hyperspectral scene from the **HYPERION** sensor: The Hermiston city scene, taken on the years 2004 and 2007 with the HYPERION sensor over the Hermiston City area (Oregon) whose spatial dimensions are 390 x 200 pixels and includes 242 spectral bands. 5 types of changes related to crop transitions are identified in this scene.

- 2018.[Wang Q, Yuan Z, Du Q, et al. GETNET: A general end-to-end 2-D CNN framework for hyperspectral image change detection](https://drive.google.com/file/d/1cWy6KqE0rymSk5-ytqr7wM1yLMKLukfP/view)   
This dataset has two hyperspectral images, which were acquired on May 3, 2013, and December 31, 2013, respectively in Jiangsu province, China. It has a size of 463×241 pixels, with 198 bands available after noisy band removal. In the ground-truth map, white pixels represent changed portions and black pixels mean unchanged parts.

### 1.3 CV

- 2014.[CDnet](http://changedetection.net/)   
A video database for testing change detection algorithms.

- 2015.[Sakurada K, Okatani T. Change Detection from a Street Image Pair using CNN Features and Superpixel Segmentation](http://www.vision.is.tohoku.ac.jp/us/research/4d_city_modeling/pano_cd_dataset/)   
This dataset consists of two subsets, named "TSUNAMI" and "GSV"."TSUNAMI" consists of one hundred panoramic image pairs of scenes in tsunami-damaged areas of Japan. "GSV consists of one hundred panoramic image pairs of Google Street View. The size of these images is 224 × 1024 pixels.

## 2 Code

### 2.1 Multispectral

#### 2.1.1 Traditional Method 
- 2019.[Bobholamovic/ChangeDetectionToolbox](https://github.com/Bobholamovic/ChangeDetectionToolbox)

- 2019.[M J Canty. Image Analysis, Classification and Change Detection in Remote Sensing(Fourth Revised Edition)](https://github.com/mortcanty/CRC4Docker)

- 2017.[M J Canty. Change Detection with Google Earth Engine Imagery](https://github.com/mortcanty/earthengine)

- 2014.[M J Canty. Image Analysis, Classification and Change Detection in Remote Sensing(Third Revised Edition)](https://github.com/mortcanty/CRCPython)

- [Zhu Zhe.Algorithm developed for Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data](https://github.com/GERSL/CCDC)

- Implementation of " [2009.Celik T. Unsupervised change detection in satellite images using principal component analysis and k-means clustering](https://ieeexplore.ieee.org/abstract/document/5196726/) ".  
[Matlab](https://github.com/rulixiang/ChangeDetectionPCAKmeans), [Python](https://github.com/abhijeet3922/Change-Detection-in-Satellite-Imagery)

- 2007.[Allan Aasbjerg Nielsen.IR-MAD(The Regularized Iteratively Reweighted Multivariate Alteration Detection)](http://people.compute.dtu.dk/alan/software.html)


#### 2.1.2 Deep Learning
- 2020.[neverstoplearn/remote_sensing_change_detection](https://github.com/neverstoplearn/remote_sensing_change_detection)
  
- 2020.[Chen J, Yuan Z, Peng J, et al. DASNet: Dual attentive fully convolutional siamese networks for change detection of high resolution satellite images](https://github.com/lehaifeng/DASNet)

- 2019.[Maria Papadomanolaki, et al. Detecting Urban Changes with Recurrent Neural Networks from Multitemporal Sentinel-2 Data](https://github.com/granularai/ChangeDetection)

- 2019.[Du B, Ru L, Wu C, et al. DSFANet (Deep Slow Feature Analysis Network)](https://github.com/rulixiang/DSFANet)

- 2019.[Peng D, Zhang Y, Guan H. End-to-End Change Detection for High Resolution Satellite Images Using Improved UNet++](https://github.com/daifeng2016/End-to-end-CD-for-VHR-satellite-image)

- 2018.[Rahman F, Vasu B, Van Cor J, et al. Siamese Network with Multi-level Features for Patch-based Change Detection in Satellite Imagery](https://github.com/vbhavank/Siamese-neural-network-for-change-detection)

- 2018.[Rodrigo Caye Daudt. Fully convolutional change detection](https://github.com/rcdaudt/fully_convolutional_change_detection)
  
- 2018.[Enqiang Guo, Xinsha Fu, et al.Learning to Measure Changes: Fully Convolutional Siamese Metric Networks for Scene Change Detection](https://github.com/gmayday1997/SceneChangeDet)

- 2018.[Shishira R Maiya,et al.Slum Segmentation and Change Detection: A Deep Learning Approach](https://github.com/cbsudux/Mumbai-slum-segmentation)

- 2016.[El Amin A M, Liu Q, Wang Y. Convolutional neural network features based change detection in satellite images](https://github.com/vbhavank/Unstructured-change-detection-using-CNN)



### 2.2 SAR

- 2019.[Feng Gao.Sea ice change detection in SAR images based on convolutional-wavelet neural networks(Matlab)](https://github.com/summitgao/SAR_Change_Detection_CWNN)

- 2019.[Feng Gao.Transferred deep learning for sea ice change detection from synthetic aperture radar images(Matlab)](https://github.com/summitgao/SAR-Change-Detection-MLFN)
  
- 2015.[Knut Conradsen, et al.Change detection in polarimetric SAR images in Python](https://github.com/fouronnes/SAR-change-detection)


## 3 Paper
**coming soon**


## 4.Contest

- [**xView 2 Building Damage Asessment Challenge**](https://xview2.org) *(DIUx, Nov 2019)*  
550k building footprints & 4 damage scale categories, 20 global locations and 7 disaster types (wildfire, landslides, dam collapses, volcanic eruptions, earthquakes/tsunamis, wind, flooding), Worldview-3 imagery (0.3m res.), pre-trained baseline model. Paper: [Gupta et al. 2019](https://arxiv.org/abs/1911.09296)

- [**遥感图像稀疏表征与智能分析竞赛-变化检测赛道**](http://rscup.bjxintong.com.cn/#/theme/4) *(Wuhan University,et al. Jul 2019)*   
本项竞赛以光学遥感图像为处理对象，参赛队伍使用主办方提供的遥感图像进行建筑物变化检测，主办方根据评分标准对变化检测结果进行综合评价。竞赛中将提供两个不同时间获取的大尺度高分辨率遥感图像（包含蓝、绿、红和近红外四个波段），以及图像中变化区域的二值化标注数据集。   

- [**广东政务数据创新大赛—智能算法赛**](https://tianchi.aliyun.com/competition/entrance/231615/introduction) *(Alibaba,et al. Nov 2017)*    
使用2015年和2017年分别获取到的广东省某地的Quickbird卫星影像（包含蓝、绿、红和近红外四个波段），识别出两年之间新增的人工地上建筑物（不包括道路）。获胜团队的解决方案可以在[天池](https://tianchi.aliyun.com/forum/postDetail?postId=3527)官网上找到。



## Reference
- [Awesome Satellite Imagery Datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [Zhang Bin's Blog. Remote Sensing Datasets](https://zhangbin0917.github.io/2018/06/12/%E9%81%A5%E6%84%9F%E6%95%B0%E6%8D%AE%E9%9B%86/)
- The picture of this page is from [Mou L et al. 2018](https://ieeexplore.ieee.org/document/8541102)
  


