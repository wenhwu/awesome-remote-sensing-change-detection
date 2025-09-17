
# <p align=center>`Awesome Remote Sensing Change Detection`</p>
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) [![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)![Forks](https://img.shields.io/github/forks/wenhwu/awesome-remote-sensing-change-detection?style=social)![GitHub stars](https://img.shields.io/github/stars/wenhwu/awesome-remote-sensing-change-detection?style=social)![Last Commit](https://img.shields.io/github/last-commit/wenhwu/awesome-remote-sensing-change-detection.svg?style=flat&logo=github&label=Last%20Commit)[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A curated list of datasets and code repositories focused on remote sensing change detection.

# Contents

- [Datasets](#datasets)
  - [Optical Datasets](#optical-datasets)
  - [Multi-Modal and SAR Datasets](#multi-modal-and-sar-datasets)
  - [Contest Datasets](#contest-datasets)
- [Open Source Toolbox](#open-source-toolbox)
- [Reference](#reference)

# Datasets

## Optical Datasets

|Year|Task|Target| Dataset |Publication|Source|Image Pairs |Image Size|Resolution|Location|Class|
|:---|:--- |:--- | :------| :------|:----------| :-------| :-------| :----------- | :----- | :---- |
|2025|BCD|Land cover|[JL1-CD](https://github.com/circleLZY/MTKD-CD)|[arXiv2025](https://arxiv.org/pdf/2502.13407)|Jilin-1|5,000|512×512|0.5-0.75m|Multiple provinces in China|2|
|2025|SCD|Building|[EBD](https://figshare.com/articles/figure/An_Extended_Building_Damage_EBD_dataset_constructed_from_disaster-related_bi-temporal_remote_sensing_images_/25285009/2)| [JRS2025](https://spj.science.org/doi/full/10.34133/remotesensing.0733?af=R)|WorldView-3|>18,000|512×512|0.3-0.5m|Global|7|
|2024|BCD|Mine| [MineNetCD](https://huggingface.co/datasets/HZDR-FWGEL/MineNetCD256) |[TGRS2024](https://ieeexplore.ieee.org/document/10744421) |Google Earth|71,711|256×256| 1.2m |Global|2|
|2024|BCD|Building| [TUE-CD](https://github.com/RSMagneto/MSI-Net)| [TGRS2024](https://ieeexplore.ieee.org/document/10623278)|WorldView-2|1,656 |256×256| 1.8m|Turkey|2|
|2024|SCD|Cropland| [CropSCD](https://github.com/lsmlyn/CropSCD)| [TGRS2024](https://ieeexplore.ieee.org/document/10579791) |-|4,141|512×512|0.5-2m|Guangdong, China|9|
|2024|SCD|Cropland| [Hi-CNA](https://rsidea.whu.edu.cn/Hi-CNA_dataset.htm) |[ISPRS P&RS 2024](https://www.sciencedirect.com/science/article/pii/S0924271624002090) |GF-2|6,797| 512×512|0.8m|China (Hebei, Shanxi, Shandong, and Hubei) |5|
|2024|SCD|Land cover|[ChangNet](https://github.com/jankyee/ChangeNet)| [ICASSP2024](https://ieeexplore.ieee.org/document/10446592)|WayBack|31,000|1900×1200|0.3m|100 Cities in China|6|
|2023|BCD|Building| [EGY-BCD](https://github.com/oshholail/EGY-BCD)      | [GRSL2023](https://ieeexplore.ieee.org/document/10145434)      |Google Earth |6,091 | 256×256| 0.25m| Egypt|2|
|2023|BCD|Building| [HRCUS-CD](https://github.com/zjd1836/AERNet)        | [TGRS2023](https://ieeexplore.ieee.org/document/10209204)      |-|11,388 |256×256| 0.5m|Zhuhai, China|2|
|2023|BCD|Building| [SI-BU](https://vrlab.org.cn/~hanhu/projects/bcenet/)| [ISPRS P&RS 2023](https://www.sciencedirect.com/science/article/pii/S0924271623001284?via%3Dihub)|Google Earth|4,932|512×512| 0.2m| Guiyang, China|2|
|2023|SCD|Land cover|[CNAM-CD](https://github.com/Silvestezhou/CNAM-CD)| [RS2023](https://www.mdpi.com/2072-4292/15/9/2464)|Google Earth|2,503|512×512|0.5m|12 State-level New Areas in China|6|
|2023|SCD|Land cover| [WUSU](https://rsidea.whu.edu.cn/resource_wusu_sharing.htm)| [IJDE2023](https://www.tandfonline.com/doi/full/10.1080/17538947.2023.2246445) |GF-2|3| 6358×6382, 7025×5500| 1m |Wuhan, China|12|
|2023|BCD|Landslide| [GVLM](https://github.com/zxk688/GVLM)| [ISPRS P&RS 2023](https://www.sciencedirect.com/science/article/pii/S0924271623000242)|Google Earth|17| 1748×1748-10808×7424|0.59m|Global|2|
|2023|SCD|Building|[BANDON](https://github.com/fitzpchao/BANDON)| [Sci. China Inf. Sci. 2023](https://link.springer.com/article/10.1007/s11432-022-3691-4) |Google Earth, Microsoft Virtual Earth, and ArcGIS|2,283|2048×2048| 0.6m|China (Beijing, Shanghai, Wuhan, Shenzhen, Hong Kong, and Jinan)|6|
|2023|SCD|Land cover| [DynamicEarthNet](https://mediatum.ub.tum.de/1650201) | [CVPR2022](https://openaccess.thecvf.com/content/CVPR2022/html/Toker_DynamicEarthNet_Daily_Multi-Spectral_Satellite_Dataset_for_Semantic_Change_Segmentation_CVPR_2022_paper.html) |PlanetFusion|54,750| 1024×1024|3m|Global|7|
|2022|BCD|Cropland| [CLCD](https://github.com/liumency/CropLand-CD)| [JSTARS2022](https://ieeexplore.ieee.org/document/9780164)|GF-2|600| 512×512|0.5-2m|Guangdong, China|2|
|2022|RSICC|Building | [LEVIR-CC](https://github.com/Chen-Yang-Liu/RSICC)  | [TGRS2022](https://ieeexplore.ieee.org/document/9934924)|Google Earth|10,077| 1024×1024| 0.5m| Texas, USA|2|
|2022|BCD|Land cover | [SYSU-CD](https://github.com/liumency/SYSU-CD)    | [TGRS2021](https://ieeexplore.ieee.org/document/9467555) |-|20,000| 256×256 | 0.5m |Hong Kong, China |2|
|2022|SCD|Building| [S2Looking](https://github.com/S2Looking/Dataset)|[RS2021](https://www.mdpi.com/2072-4292/13/24/5094) |GF, SuperView, BJ-2|5,000| 1024×1024| 0.5-0.8m| Global|2|
|2022|BCD|Building| [LEVIR-CD+](https://github.com/S2Looking/Dataset)|[RS2021](https://www.mdpi.com/2072-4292/13/24/5094) |Google Earth|985|1024×1024|0.5m|Texas, USA|2|
|2022|SCD|Land cover| [Landsat-SCD](https://figshare.com/articles/figure/Landsat-SCD_dataset_zip/19946135/1)|[IJDE2022](https://www.tandfonline.com/doi/full/10.1080/17538947.2022.2111470) |Landsat|8,468|416×416|30m|Xinjiang, China|10|
|2022|SCD|Building|[NanjingDataset](https://github.com/SianGIS/NanjingDataset)|[ISPRS P&RS 2022](https://www.sciencedirect.com/science/article/pii/S0924271622001344) |Google Earth|2,519|256×256|0.3m|Nanjing, China|3|
|2021|SCD|Land cover| [S2MTCP](https://zenodo.org/records/4280482)|[ICPR2021](https://link.springer.com/chapter/10.1007/978-3-030-68787-8_42) |Sentinel-2|1,520|600×600|10m|Global|-|
|2021|BCD|Urban|[HTCD](https://github.com/ShaoRuizhe/SUNet-change_detection) |[RS2021](https://www.mdpi.com/2072-4292/13/18/3750/htm)|Google Earth, Open Aerial Map|3,772|256×256, 2048×2048|0.5971m, 0.07465m|Chisinau, Moldova|2|
|2020|BCD|Building| [CD_Data_GZ](https://github.com/daifeng2016/Change-Detection-Dataset-for-High-Resolution-Satellite-Imagery)|[TGRS2020](https://ieeexplore.ieee.org/document/9161009)|Google Earth|19| 1006×1168-4936×5224| 0.55m| Guangzhou, China|2|
|2020|BCD|Building| [DSIFN](https://github.com/GeoZcx/A-deeply-supervised-image-fusion-network-for-change-detection-in-remote-sensing-images/tree/master/dataset)|[ISPRS P&RS 2020](https://www.sciencedirect.com/science/article/pii/S0924271620301532?via%3Dihub) |Google Earth|3,940 | 512×512|-|China (Beijing, Chengdu, Shenzhen, Chongqing, Wuhan, and Xian)|2|
|2020|BCD|Building| [LEVIR-CD](https://justchenhao.github.io/LEVIR/)| [RS2020](https://www.mdpi.com/2072-4292/12/10/1662)|Google Earth|637| 1024×1024|0.5m|Texas, USA|2|
|2020|SCD|Land cover| [Hi-UCD](https://github.com/Daisy-7/Hi-UCD-S?tab=readme-ov-file)|[arXiv2020](https://arxiv.org/abs/2011.03247) |Aerial Images|1,293|1024×1024|0.1m|Tallinn, Estonia|9|
|2020|SCD|Land cover| [SECOND](https://captain-whu.github.io/SCD/)| [TGRS2021](https://ieeexplore.ieee.org/document/9555824) |Aerial Images |4,662|512×512| -  |China (Hangzhou, Chengdu, and Shanghai)|6|
|2019|SCD|Land cover| [HRSCD](https://ieee-dataport.org/open-access/hrscd-high-resolution-semantic-change-detection-dataset)| [CVIU2019](https://www.sciencedirect.com/science/article/pii/S1077314219300992) |IGN|291|10000×10000|0.5m|France (Rennes, and Caen)|5|
|2018|BCD|Building| [WHU-CD](https://study.rsgis.whu.edu.cn/pages/download/building_dataset.html)| [TGRS2018](https://ieeexplore.ieee.org/document/8444434)|Aerial Image|1| 32507×15354|0.2m| Christchurch, New Zealand|2|
|2018|BCD|Building| [CDD](https://drive.google.com/file/d/1GX656JqqOyBi_Ef0w65kDGVto-nHrNs9/edit?pli=1)| [Int. Arch. Photogramm. Remote Sens. Spatial Inf. 2018](https://isprs-archives.copernicus.org/articles/XLII-2/565/2018/isprs-archives-XLII-2-565-2018.pdf) |Google Earth|1,6000| 256×256| 0.03-1m |-|2|
|2018|BCD|Riverway| [The River Data Set](https://share.weiyun.com/5xdge4R)|[TGRS2018](https://ieeexplore.ieee.org/document/8418840)|EO-1 Hyperion|1|463×241|30m|Jiangsu, China|2|
|2018|BCD|Land cover|[OSCD](https://ieee-dataport.org/open-access/oscd-onera-satellite-change-detection)|[IGARSS2018](https://ieeexplore.ieee.org/document/8518015)|Sentinel-2|24|600×600|10-60m|Global|2|
|2008|BCD|Land cover|[SZTAKI](http://web.eee.sztaki.hu/remotesensing/airchange_benchmark.html)|[TGRS2009](https://ieeexplore.ieee.org/document/5169964)|Aerial Images|13|952x640|1.5m|-|


## Multi-Modal and SAR Datasets

|Year|Task|Target| Dataset |Publication|Source|Image Pairs |Image Size|Resolution|Location|Class|
|:---|:---|:--- | :------| :------|:----------| :-------| :-------| :----------- | :----- | :---- |
|2025|SCD|Building| [BRIGHT](https://github.com/ChenHongruixuan/BRIGHT) | [arXiv2025](https://arxiv.org/abs/2501.06019) |Optical and SAR|4,538| 1024×1024| 0.3-1m|Global|4|
|2024|SCD|Building| [Hi-BCD](https://github.com/HATFormer/MMCD) | [Information Fusion 2023](https://www.sciencedirect.com/science/article/pii/S1566253524001362) |Aerial Images, DSMs|1,500| 1000×1000 |0.25m |Netherlands (Amsterdam, Rotterdam, and Utrecht)|3|
|2024|SCD|Flood |[UrbanSARFloods](https://github.com/jie666-6/UrbanSARFloods)|[CVPRW2024](https://openaccess.thecvf.com/content/CVPR2024W/EarthVision/html/Zhao_UrbanSARFloods_Sentinel-1_SLC-Based_Benchmark_Dataset_for_Urban_and_Open-Area_Flood_CVPRW_2024_paper.html) | Sentinel-1|8,879| 512×512|20m|Global|5|
|2024|SCD|Land use |[EVLab-CMCD](https://github.com/whudk/EVLab-CMCD) | [ISPSR P&RS 2024](https://www.sciencedirect.com/science/article/pii/S0924271624003873)|GF-2, BJ-2, Historical land use maps|5,622|512×512| 0.8m| 10 Cities in China|13|
|2023|BCD|Flood |[CAU-Flood](https://github.com/CAU-HE/CMCDNet)| [JAG2023](https://www.sciencedirect.com/science/article/pii/S1569843223000195) |Sentinel-1, Sentinel-2|18,302| 256×256|10m|Global|2|
|2023|SCD|Flood|[Kuro Siwo](https://github.com/Orion-AI-Lab/KuroSiwo)|[NeurIPS2024](https://proceedings.neurips.cc/paper_files/paper/2024/hash/43612b0662cb6a4986edf859fd6ebafe-Abstract-Datasets_and_Benchmarks_Track.html)|Sentinel-1, DEM| 67,490 |224×224| 10m|Gloabl|3|
|2023|SCD|Urban|[SMARS](https://www.dlr.de/en/eoc/about-us/remote-sensing-technology-institute/photogrammetry-and-image-analysis/public-datasets/smars)| [ISPRS P&RS 2023](https://www.sciencedirect.com/science/article/pii/S092427162300254X)|Simulated Orthoimages and DSMs|-|512×512|0.3m, 0.5m|Simulated Paris and Venice|3|
|2023|BCD|Urban|[3DCD](https://sites.google.com/uniroma1.it/3dchangedetection/home-page?pli=1) |[ISPRS P&RS 2023](https://www.sciencedirect.com/science/article/pii/S0924271622003240)|Aerial Images, DSMs|472|400×400, 200×200|0.5m, 1m|Valladolid, Spain|2| 
|2023|SCD|Urban|[Urb3DCD–V2](https://ieee-dataport.org/open-access/urb3dcd-urban-point-clouds-simulated-dataset-3d-change-detection)|[ISPRS P&RS 2023](https://www.sciencedirect.com/science/article/pii/S0924271623000394)|ALS, Multi-Sensor|-|-|-|Simulated|7|
|2022|BCD|Flood| [Wuhan](https://github.com/GeoZcx/A-Domain-Adaption-Neural-Network-for-Change-Detection-with-Heterogeneous-Optical-and-SAR-Remote-Sens/tree/main/data) | [JAG2022](https://www.sciencedirect.com/science/article/pii/S0303243422000952) |Sentinel-2, COSMO-SkyMed|1| 11216×13693|3m |Wuhan, China|2|
|2022|BCD|Flood|[Ombria](https://github.com/geodrak/OMBRIA) |[JSTARS2022](https://ieeexplore.ieee.org/document/9723593/) |Sentinel-1, Sentinel-2| 1,688| 256×256| 10m|Global|2|
|2021|BCD|Land cover|[MultiModalOSCD](https://github.com/PatrickTUM/multimodalCD_ISPRS21)|[ISPRS. XXIV ISPRS Congress 2021](https://isprs-archives.copernicus.org/articles/XLIII-B3-2021/243/2021/isprs-archives-XLIII-B3-2021-243-2021.pdf)|Sentinel-1, Sentinel-2|24|600×600|10-60m|Global|2|


## Contest Datasets

| Year | Target | Contest | Track | Image Pairs | Image Size | Resolution |Other|
| --- | --- | --- | --- | --- | --- | --- | --- |
| 2024 | Land cover| [2024 ISPRS第一技术委员会多模态遥感应用算法智能解译大赛](https://www.gaofen-challenge.com/challenge) |基于高分辨率可见光图像的感兴趣区域内部变化智能检测| 4,000 | 512×512 | 2m |-|
| 2024 | Land cover | [2024“吉林一号”杯卫星遥感应用青年创新创业大赛](https://www.jl1mall.com/contest/matchMenu) |高分辨率遥感影像全要素变化检测研究| 5,000 | 512×512 |<0.75m|-|
| 2023 | Cropland | [2023“吉林一号”杯卫星遥感应用青年创新创业大赛](https://www.jl1mall.com/contest/match/info?id=1645664411716952066) |基于高分辨率卫星影像的耕地变化检测| 8,000 | 256×256 |<0.75m|-|
| 2023 | Land cover | [2023“国丰东方慧眼杯”遥感影像智能处理算法大赛](http://rsipac.whu.edu.cn/) |对象级变化检测| >6,000 | 512×512 | 1-2m |-|
| 2022 | Land cover | [2022“航天宏图杯”遥感影像智能处理算法大赛](http://rsipac.whu.edu.cn/) |遥感影像变化检测| >6,000 | 512×512 | 1-2m |-|
| 2022 | Flood | [SpaceNet8: Flood Detection Challenge](https://join.topcoder.com/spacenet) | Flood Detection Challenge Using Multiclass Segmentation | 12 | 1300×1300 | 0.3-0.8m |[Dataset Paper](https://openaccess.thecvf.com/content/CVPR2022W/EarthVision/papers/Hansch_SpaceNet_8_-_The_Detection_of_Flooded_Roads_and_Buildings_CVPRW_2022_paper.pdf), [Solution Paper](https://ieeexplore.ieee.org/document/10281500)|
| 2021 |Land cover|[2021 IEEE GRSS Data Fusion Contest](https://www.grss-ieee.org/community/technical-committees/2021-ieee-grss-data-fusion-contest-track-msd/)|Multitemporal Semantic Change Detection|2,250|-|-|[Outcome Paper](https://ieeexplore.ieee.org/document/9690575)|
| 2021 |Land cover|[2021 DynamicEarthNet Challenge](https://codalab.lisn.upsaclay.fr/competitions/2882) | Weakly-Supervised Unsupervised Binary Land Cover Change Detection, Multi-Class Change Detection|54,750|1024x1024|3.0|[Top1 Solution](https://github.com/solcummings/earthvision2021-weakly-supervised), [Dataset Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Toker_DynamicEarthNet_Daily_Multi-Spectral_Satellite_Dataset_for_Semantic_Change_Segmentation_CVPR_2022_paper.pdf)|
| 2021 | Land cover | [2021 “昇腾杯”遥感影像智能处理算法大赛](http://rsipac.whu.edu.cn/subject_two_2021) | 耕地建筑物变化检测 | >6,000 | 512×512 | 1-2m |[Top4 Solution](https://github.com/WangZhenqing-RS/2021rsipac_changeDetection_TOP4), [Top5 Solution](https://github.com/78666621/2021rsipac_changeDetection_TOP5)|
| 2021 | Building | [遥感图像智能解译技术挑战赛](https://captain-whu.github.io/PRCV2021_RS/tasks.html) | 遥感图像建筑物变化检测 | 10,000 | 512×512 | - |-|[Top2 Solution](https://github.com/businiaoo/PRCV2021-Change-Detection-Contest-2nd-place-Solution), [Top3 Solution](https://github.com/likyoo/PRCV2021_ChangeDetection_Top3)|
| 2021 | Building | [2021 慧眼“天智杯”人工智能挑战赛](https://rsaicp.com/portal/contestList) |可见光建筑智能变化检测| 5,000 | 1024×1024 | 0.5-0.7m |-|
| 2020 | Land cover | [2020 商汤科技首届AI遥感解译大赛](https://senseearth-cloud.com/) |变化检测|4,662 | 512×512 | 0.5-3m |[Top1 Solution](https://github.com/LiheYoung/SenseEarth2020-ChangeDetection)|
| 2020 | Land cover | [SpaceNet 7: Multi-Temporal Urban Development Challenge](https://medium.com/the-downlinq/the-spacenet-7-multi-temporal-urban-development-challenge-dataset-release-9e6e5f65c8d5) | Multi-Temporal Urban Development Challenge |-|-| 4m |[Solutions](https://github.com/SpaceNetChallenge/SpaceNet7_Multi-Temporal_Solutions), [Dataset Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Van_Etten_The_Multi-Temporal_Urban_Development_SpaceNet_Dataset_CVPR_2021_paper.pdf)|
| 2019 | Building | [xView2 Challenge](https://xview2.org/dataset) | Building Damage Assessment | 11,034 | 1024×1024 | - |[Dataset Paper](https://arxiv.org/abs/1911.09296)|

# Open Source Toolbox

| Year | Abbreviation | Description | Last Commit|GitHub Stars|
| :--- | :--- | :--- | :--- | :--- | 
|2024|[torchange](https://github.com/Z-Zheng/pytorch-change-models)| A benchmark library providing out-of-box, straightforward implementations of contemporary spatiotemporal change detection models, metrics, and datasets to promote reproducibility in remote sensing research. |![Last Commit](https://img.shields.io/github/last-commit/Z-Zheng/pytorch-change-models.svg?style=flat&logo=github&label=Last%20Commit)|![GitHub stars](https://img.shields.io/github/stars/Z-Zheng/pytorch-change-models?style=social)|
|2022| [Open-CD](https://github.com/likyoo/open-cd)|The most comprehensive open-source toolbox for change detection, offering a unified platform with diverse methods, training/inference tools, data analysis scripts, and benchmarks to support research and development in the field. Paper: [arXiv2024](https://arxiv.org/abs/2407.15317). |![Last Commit](https://img.shields.io/github/last-commit/likyoo/open-cd.svg?style=flat&logo=github&label=Last%20Commit)|![GitHub stars](https://img.shields.io/github/stars/likyoo/open-cd?style=social)|
|2022|[PaddleRS](https://github.com/PaddlePaddle/PaddleRS)| A remote sensing toolkit based on PaddlePaddle that supports change detection among other tasks, providing dedicated models (e.g., BIT, FarSeg), large-image processing capabilities, and practical tutorials for analyzing temporal land cover differences. The PyTorch version is called [CDLab](https://github.com/Bobholamovic/CDLab).|![Last Commit](https://img.shields.io/github/last-commit/PaddlePaddle/PaddleRS.svg?style=flat&logo=github&label=Last%20Commit)|![GitHub stars](https://img.shields.io/github/stars/PaddlePaddle/PaddleRS?style=social)|
|2020|[Change Detection Repository](https://github.com/ChenHongruixuan/ChangeDetectionRepository)|It provides Python implementations of selected traditional change detection methods (e.g., CVA, SFA, MAD) and deep learning-based approaches (e.g., SiamCRNN, DSFA, and FCN-based methods).|![Last Commit](https://img.shields.io/github/last-commit/ChenHongruixuan/ChangeDetectionRepository.svg?style=flat&logo=github&label=Last%20Commit)|![GitHub stars](https://img.shields.io/github/stars/ChenHongruixuan/ChangeDetectionRepository?style=social)|

## Reference

- [daifeng2016/Awesome-Optical-Remote-Sensing-Datasets-and-Methods](https://github.com/daifeng2016/Awesome-Optical-Remote-Sensing-Datasets-and-Methods?tab=readme-ov-file)
- [chrieke/awesome-satellite-imagery-datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [MinZHANG-WHU/Change-Detection-Review](https://github.com/MinZHANG-WHU/Change-Detection-Review)
