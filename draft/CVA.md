# Change Vector Analysis

## 1. CVA's fundamental?

变化向量是描述从时相1到时相2变化的方向和大小的光谱变化向量, 如图1(a)。

![图1](./img/CVA/1.PNG)

设时相$t_1$ , $t_2$图像的像元灰级矢量分别为$G =(g_1 , g_2 , …, g_k)^T$和$H =(h_1 , h_2 , … , h_k)^T$, 则变化向量为:
$$
    ΔG = G-H =
    \begin{pmatrix}
    g_1 -h_1 \\
    g_2 -h_2 \\
    \vdots \\
    g_k -h_k \\
    \end{pmatrix}
$$
　ΔG包含了两幅图像中所有变化信息, 变化强度由‖ΔG‖决定:
$$ ‖ΔG‖ = \sqrt{(g_1-h_1)^2+(g_2-h_2)^2+{\cdots}+(g_k-h_k)^2} $$
按照变化强度‖ΔG‖的定义，不难发现‖ΔG‖越大, 表明图像的差异越大, 变化发生的可能性越大。因此, 判断变化和非变化像元, 可根据变化强度‖ΔG‖的大小设定阈值来实现。即像元‖ΔG‖超过某一阈值时, 即可判定为土地利用/覆盖发生变化的像元。变化的类型可由ΔG的指向确定。例如, 图1(b)说明变化没有发生或不能被探测到, 因为变化强度没有超过阈值；而图1(c), (d)则说明不同类型的变化已经发生。

**Reference**

[基于变化向量分析的土地利用/覆盖变化动态监测(Ⅰ)—变化阈值的确定方法](http://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFD2001&filename=YGXB200104003&uid=WEEvREdxOWJmbC9oM1NjYkZCbDZZZ21mamloRUR5WGRBa3gyS1lvb2V0MUs=$R1yZ0H6jyaa0en3RxVUd8df-oHi7XMMDo7mtKT6mSmEvTuk11l2gFA!!&v=MTk4MjV4WVM3RGgxVDNxVHJXTTFGckNVUkxLZVp1Wm1GeS9rVUwvS1BDclRiTEc0SHRETXE0OUZaNFI4ZVgxTHU=)

## 2. CVA's advantage?

变化向量法由于不仅可以避免分类后比较法多次分类费时费力, 误差累积并出现不合理变化类型(如城市变为水田)的缺陷, 而且与其它像元光谱的直接比较方法相比, 可以利用较多甚至全部的波段来探测变化像元, 并提供变化像元的类型信息。

**Reference**

[基于变化向量分析的土地利用/覆盖变化动态监测(Ⅰ)—变化阈值的确定方法](http://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFD2001&filename=YGXB200104003&uid=WEEvREdxOWJmbC9oM1NjYkZCbDZZZ21mamloRUR5WGRBa3gyS1lvb2V0MUs=$R1yZ0H6jyaa0en3RxVUd8df-oHi7XMMDo7mtKT6mSmEvTuk11l2gFA!!&v=MTk4MjV4WVM3RGgxVDNxVHJXTTFGckNVUkxLZVp1Wm1GeS9rVUwvS1BDclRiTEc0SHRETXE0OUZaNFI4ZVgxTHU=)

## 3. CVA's disadvantage?

1. **数据质量和预处理要求较高。** 由于土地利用/覆盖变化信息和各种不同时相间传感器、物候、大气条件和土壤水分等差异导致的“干扰噪声”信息常常同时被探测到, 从而导致混淆和错判。因此, 变化向量分析方法要求进行较为严格的辐射校正, 事实上, 目前对各种干扰(尤其是物候)导致的辐射差异的校正方法仍不成熟, 因此, 只能通过选择同一传感器、同一时相的数据来最大可能的减小“干扰噪声”。这种对数据和预处理的过高要求极大地限制了变化向量分析方法的广泛使用。

2. **缺乏高效的变化阈值确定方法。** 变化阈值的确定是变化向量分析法成功使用的关键。现有的研究常常根据经验确定变化阈值, 划分出变化和非变化像元。所以, 变化阈值的确定一般是主观的, 需要经过较长时间的摸索。

3. **随着利用波段的增加,变化类型判断难度加大。** 现有研究中对变化类型的判定基本上归纳为3种方法:二维空间向量的三角函数法[1], 高于二维空间的波段符号组合法[2], 多时相空间的主成分分析法[3]。在多数CVA的应用中, 变化类型的判断主要通过每个计算波段的“+”、“-”符号组合(+代表增加, -代表减少)结合目视解译进行。但当应用这种常规的符号组合方法判断变化类型时, 常常出现两个问题:
   - 一是当计算波段数为n时, 组合法只能表示$2^n$种符号。如果某一区域中有m种土地利用/覆类类型并且各种土地利用/覆盖变化都可能发生, 那么该区域土地利用/覆盖变化类型的总数就是m*(m-1),因此, 很有可能出现一种符号组合代表多种土地利用/覆盖变化类型的情况, 从而导致对变化类型的错误判断。
   - 二是随着计算波段的增加, 符号组合将呈几何级数增加, 变化类型判断难度很大。

**Reference**

[基于变化向量分析的土地利用/覆盖变化动态监测(Ⅰ)—变化阈值的确定方法](http://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFD2001&filename=YGXB200104003&uid=WEEvREdxOWJmbC9oM1NjYkZCbDZZZ21mamloRUR5WGRBa3gyS1lvb2V0MUs=$R1yZ0H6jyaa0en3RxVUd8df-oHi7XMMDo7mtKT6mSmEvTuk11l2gFA!!&v=MTk4MjV4WVM3RGgxVDNxVHJXTTFGckNVUkxLZVp1Wm1GeS9rVUwvS1BDclRiTEc0SHRETXE0OUZaNFI4ZVgxTHU=)

[基于变化向量分析(CVA)的土地利用/覆盖变化动态监测(Ⅱ)—变化类型的确定方法](http://kns.cnki.net/KCMS/detail/detail.aspx?dbcode=CJFQ&dbname=CJFD2001&filename=YGXB200105004&uid=WEEvREdxOWJmbC9oM1NjYkZCbDZZZ21mamloRUR5WGRBa3gyS1lvb2V0MUs=$R1yZ0H6jyaa0en3RxVUd8df-oHi7XMMDo7mtKT6mSmEvTuk11l2gFA!!&v=MDk2OTMzcVRyV00xRnJDVVJMS2VadVptRnkva1ViN0tQQ3JUYkxHNEh0RE1xbzlGWUlSOGVYMUx1eFlTN0RoMVQ=)

1. [Malila W A. Change vector analysis:An approach for detecting forest change with Landsat](https://docs.lib.purdue.edu/cgi/viewcontent.cgi?referer=https://cn.bing.com/&httpsredir=1&article=1386&context=lars_symp)
2. [Virag L A, Colwell J E. An Improved Procedure for Analysis of Change in Thematic Mapper Image-Pairs]()
3. [Lambin E , Strahler. A Change-vector analysis in multitemporal space:a tool to detect and categorize land-cover change processing using high temporal-resolution satellite data](https://www.sciencedirect.com/science/article/abs/pii/0034425794901449)