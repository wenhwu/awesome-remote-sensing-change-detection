# Binary change detection

## 1. the key of the binary change detection?

Well-known transformation techinques successfully applied to change detection are **[canonical correlation](https://ieeexplore.ieee.org/document/988962)**, **[Principal Component Analysis (PCA)](https://ieeexplore.ieee.org/document/5196726/)** and **[Independent Component Analysis (ICA)](https://ieeexplore.ieee.org/document/5418265)**. In [1], PCA is applied to the diﬀerence image and changes are recognized as the ﬁrst few principal components. In [2], an orthogonal(正交的) representation of the changes based on the Gram-Schmidt procedure was used. In [3], the tasselled cap transformation（穗帽变换）was applied to detect the vegetation change from Landsat images. It is worth mentioning also the **[Multivariate Alteration Detection (MAD) technique](http://www.forskningsdatabasen.dk/en/catalog/2389479123)**, which is based on the [canonical correlation analysis](https://ieeexplore.ieee.org/document/988962). An improved version named **[Iterative Reweighted MAD (IR-MAD)](https://ieeexplore.ieee.org/document/4060945)** was proposed to provide more reliable output components thus emphasizing changes.

* However, the main disadvantage of the above mentioned transformation-based CD approaches is that they require a strong interaction with the end-users（终端用户）to select the most informative components emphasizing the speciﬁc changes of interest, which is usually time consuming.
* On the other hand, the transformation-based methods do not provide a clear number of changes. The number of detected changes highly depends on the selected number of components and the change information represented in those components. Some changes might be still mixed and unidentiﬁed in a given component.

Therefore, the transformation-based approaches are good at extracting features for enhancing the detection of speciﬁc kinds of changes in CD, but in general they are not suitable for detecting all the possible change classes.

**Reference**

[Zanetti, M. (2017). Advanced methods for the analysis of multispectral and multitemporal remote sensing images (Doctoral dissertation, University of Trento)](http://eprints-phd.biblio.unitn.it/2041/)

1. [Change detection using principal component analysis and fuzzy set theory](https://www.tandfonline.com/doi/abs/10.1080/07038992.1993.10855147)
2. [Change detection using the Gramm-Schmidt transformation applied to mapping forest mortality](https://www.sciencedirect.com/science/article/abs/pii/0034425794900760)
3. [A comparison of methods for monitoring multitemporal vegetation change using Thematic Mapper imagery](https://www.sciencedirect.com/science/article/pii/S0034425701002966)