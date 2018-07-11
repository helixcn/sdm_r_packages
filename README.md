# sdm_r_packages

## 前 言

自从BIOMOD程序包在CRAN发布以来，众多的生态学家将注意力集中到R。

这是因为：

1. 用R语言开发软件包相对容易，R中的数据对象类型容易学习和理解，数据读取等也非常容易。

2. 近些年诞生的一些R程序包，让R十分方便地处理shape文件和raster文件等， 这就让物种生态位建模中加载环境图层，读写其他软件安生成的文件以及保存结果非常方便。

3. 绘图R的优势之一，用户一般不需要特别复杂的编程，就可以生成精美的图形，而物种生态位模型研究中用图形展示结果非常重要。

4. 计算性能方面，R程序可以与C或C++写的代码完美结合，客服了计算瓶颈。这就让物种生态位模型中常用的random forest, boosted regression trees, randomization test, cross validation, bootstrap等都能在可接受的时间内完成。

5. R本身有较为完备的文档系统，近几年诞生的knitr, Rmarkdown等程序包， 让编写软件包指南变得非常容易。有了良好的文档系统， 用户也更容易学习和使用R程序包。

6. R拥有庞大的用户群，通过R-sig邮件组, github以及stackoverflow等网站用户可以很快找到大部分问题的解决方案，其中当然也包括很多物种分布区模型预测相关的问题。

物种生态位建模的程序包很多，大部分在CRAN集中保存。不过CRAN上的程序包已经超过12000个，虽然CRAN task view已经按照程序包所属的类别分别做了介绍， 但是目前仍然没有一个专门针对物种生态位模型的CRAN task view。这些程序包混在这12000多个程序包中，有时难以寻找。 为此，本人整理了CRAN或者github上与物种生态位模型分析相关的程序包列表，希望能反映近几年的最新进展，以方便相关工作人员查找和使用。

由于掌握的信息有限，难免有很多错漏，望读者提出宝贵意见。


## 物种分布模型相关的R程序包列表

* [`adehabitatHS`](https://cran.r-project.org/web/packages/adehabitatHS) :分析动物栖息地
* [`adespatial`](https://cran.r-project.org/web/packages/adespatial): 多元、多尺度物种分布空间分析， 维护者是Stephane Dray, 该程序包中的forward.sel函数与packfor包功能相似
* [`ALA4R`](https://cran.r-project.org/web/packages/ALA4R):查询澳大利亚The Atlas of Living Australia (ALA) 网站动植物分布记录
* [`BIEN`](https://cran.r-project.org/web/packages/BIEN):查询NCEAS的BIEN数据库， 包括物种分布记录、性状、样方数据和系统分类位置等 http://Bien.nceas.ucsb.edu/bien/
* [`biogeo`](https: //onlinelibrary.wiley.com/doi/abs/10.1111/ecog.02118):用于检查分布点数据的质量，以提高物种分布模型的准确性。
* [`biomod2`](https://cran.r-project.org/web/packages/biomod2):用于多种物种生态位模型的整合建模， 这是Wilfried Thuiller研究组开发的程序包， 是biomod的继承与发展。
* [`bossMaps`](https://cran.r-project.org/web/packages/bossMaps) :用于将基于专家意见的物种分布图(如野外手册中的分布图)转换为连续分布面数据。用于进一步校正物种分布图
* [`cocorresp`](https://cran.r-project.org/web/packages/cocorresp):基于Co-CA方法，进行群落水平的物种相关性检验
* [`coenocliner`](https://cran.r-project.org/web/packages/coenocliner):群落生态学程序包， 作者Gavin Simpson， 用于模拟环境梯度上物种出现与否及其多度。 
* [`coenoflex`](https://cran.r-project.org/web/packages/coenoflex): 蒙大拿大学David W. Roberts 开发的程序包， 用于模拟植被
* [`coexist`](https://cran.r-project.org/web/packages/coexist): 陈友华编写的物种共存分析的程序包
* [`comclim`](https://cran.r-project.org/web/packages/comclim): 群落结构与气候分析
* [`CommEcol`](https://cran.r-project.org/web/packages/CommEcol): 群落生态学数据分析
* [`ConR`](https://cran.r-project.org/web/packages/ConR): 估计物种分布区大小， 用于IUCN红色名录等级的分析
* [`cooccur`](https://cran.r-project.org/web/packages/cooccur): 分析实地调查中物种共同出现的概率
* [`CoordinateCleaner`](https://cran.r-project.org/web/packages/CoordinateCleaner): 分布数据的校验， 特别是国家与地区水平，地名与经纬度是否相符等。 https://github.com/azizka/CoordinateCleaner
* [`demoniche`](https://cran.r-project.org/web/packages/demoniche): 种群分布的空间分析
* [`dismo`](https://cran.r-project.org/web/packages/dismo): 物种生态位模型预测， 这是Robert Hijmans编写的程序包，功能繁多。作者的文档写得很清楚， 是入门的重要参考。
* [`downscale`](https://cran.r-project.org/web/packages/downscale): 基于粗尺度的物种分布区获得精细尺度的物种分布区 downscales species occupancy at coarse grain sizes to predict species occupancy at fine grain sizes (更多内容参见 http://www.meteo.unican.es/climate4R )
* [`ecolottery`](https://cran.r-project.org/web/packages/ecolottery): 用于模拟群落，可实现两种模拟，coalescent-based simulation, forward-in-time simulation
* [`EcoSimR`](https://cran.r-project.org/web/packages/EcoSimR): 群落生态学研究中的零模型， 主要用于检测物种共存，计算生态位宽度等， 统计生态学名家N. Gotelli等人开发的程序包。
* [`ecospat`](https://cran.r-project.org/web/packages/ecospat): 物种分布模型领军人物Antoine Guisan研究组开发的程序包， 用于进行空间生态学分析，特别是针对物种分布， 生态位， 群落构建等分析，有完整的工作流程 (http://www.unil.ch/ecospat/home/menuguid/ecospat-resources/tools.html)
* [`ENiRG`](https://cran.r-project.org/web/packages/ENiRG): 用R-GRASS进行物种分布区预测
* [`ENMeval`](https://cran.r-project.org/web/packages/ENMeval): 用于评估物种生态位模型，第一作者 Robert Muscarella 在群落生态学和宏生态学也有很深的造诣。
* [`ENMTools`](https://github.com/danlwarren/ENMTools/): Dan Warren 开发的R程序包， 分析物种生态位进化。
* [`EnvNicheR`](https://cran.r-project.org/web/packages/EnvNicheR): 生态位宽度和重叠
* [`FactorsR`](https://cran.r-project.org/web/packages/FactorsR): 分析影响物种丰富度的因子及各因子的贡献 
* [`fitdistrplus`](https://cran.r-project.org/web/packages/fitdistrplus): 物种多样性格局的模型与拟合
* [`fuzzySim`](https://cran.r-project.org/web/packages/fuzzySim): 物种分布区数据的模糊化处理以及分布区预测
* [`hSDM`](https://cran.r-project.org/web/packages/hSDM): 分层贝叶斯物种分布模型，该框架可使用 物种出现的01数据以及多度数据，结合生境适应性、空间关联、人为干扰以及物种被发现的容易程度进行分布区模型预测。 参考 https://onlinelibrary.wiley.com/doi/full/10.1111/ecog.02445
* [`indicspecies`](https://cran.r-project.org/web/packages/indicspecies): 基于物种多度和是否出现，计算生态位宽度等
* [`iSDM`](https://cran.r-project.org/web/packages/iSDM): 入侵物种分布模型
* [`jrich`](https://cran.r-project.org/web/packages/jrich): 进化独特性及其Jack-Knife支持率分析 Jack-Knife Support for Evolutionary Distinctiveness Indices Iand W (https`](https://link.springer.com/chapter/10.1007/978-3-319-22461-9_11)
* [`kissmig`](https://cran.r-project.org/web/packages/kissmig): 物种迁移预测
* [`KnowBR`](https://cran.r-project.org/web/packages/KnowBR): 基于物种分布数据评估某地点调查是否完整
* [`letsR`](https://cran.r-project.org/web/packages/letsR): 宏生态学研究中地理数据、物种分布数据和环境数据的处理与分析 (https://github.com/macroecology/letsR)
* [`mapr`](https://cran.r-project.org/web/packages/mapr): 利用spocc和rgbif等程序包获取的物种分布记录绘图，可生成基于leaflet的网页。
* [`MaxentVariableSelection`](https://cran.r-project.org/web/packages/MaxentVariableSelection): 评估Maxent模型预测物种分布过程中，如何选取环境因子
* [`maxlike`](https://cran.r-project.org/web/packages/maxlike): 利用极大似然方法估计物种分布区，直接生成分布概率。
* [`maxnet`](https://cran.r-project.org/web/packages/maxnet): 用glmnet进行物种分布区预测 (https://github.com/mrmaxent/maxnet)
* [`MetaLandSim`](https://cran.r-project.org/web/packages/MetaLandSim): 分析景观水平物种分布区的变化以及全球变化带来的等影响等
* [`MIAmaxent`](https://cran.r-project.org/web/packages/MIAmaxent): 用于训练和筛选Maxent模型
* [`mobsim`](https://cran.r-project.org/web/packages/mobsim): 群落物种分布和多度的空间模拟
* [`modEvA`](https://cran.r-project.org/web/packages/modEvA): 用于物种分布区模型的评估 (http://modeva.r-forge.r-project.org/)
* [`mopa`](https://cran.r-project.org/web/packages/mopa): 基于物种生态位模型预测物种是否出现 (https://github.com/SantanderMetGroup/mopa/wiki) 用Pseudo-Absences方法进行物种分布区建模， 可基于Warren et al. (2008) 的方法计算物种生态位重叠
* [`netassoc`](https://cran.r-project.org/web/packages/netassoc): 种间关联计算
* [`nicheROVER`](https://cran.r-project.org/web/packages/nicheROVER): 生态位宽度与重叠
* [`nodiv`](https://cran.r-project.org/web/packages/nodiv): 计算整合进化树和物种分布模型的两个指数 the speciﬁc overrepresentation score (SOS) and the geographic node diverg ence (GND) score (https://besjournals.onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.12283)
* [`paleobioDB`](https://cran.r-project.org/web/packages/paleobioDB): 查询PaleobioDB的记录，并进行简单可视化
* [`pez`](https://cran.r-project.org/web/packages/pez): Pearse, Cadotte, Cavender-Bares, Ives, C. Tucker, Mat Helmus 等人编写的程序包， 用于群落系统发育分析，提供若干修正的指数以及 pglmm等。
* [`phyloclim`](https://cran.r-project.org/web/packages/phyloclim): 整合气候生态位进化以及系统发育， 可计算生态位重叠等，重建祖先分类单元的气候， 分析分布区大小和分化时间的关系，用随机化方法检验两个种生态位是否相等。
* [`PresenceAbsence`](https://cran.r-project.org/web/packages/PresenceAbsence): 用于评估Presence-Absence模型的准确性，可计算confusion matrices, pcc, sensitivity, specificity, Kappa等指数并绘图等。
* [`RADanalysis`](https://cran.r-project.org/web/packages/RADanalysis): 多度分布曲线分析
* [`rangeBuilder`](https://cran.r-project.org/web/packages/rangeBuilder): 物种分布数据的整理和标准化。Occurrence Filtering, Geographic and Taxonomic Standardization and Generation of Species Range Polygons
* [`rangeMapper`](https://cran.r-project.org/web/packages/rangeMapper): 生活史性状的宏生态学分析平台，个体大小与地理分布的关系等
* [`raptr`](https://cran.r-project.org/web/packages/raptr): 确定优先保护区域， 本程序包基于商业软件Gurobi http://www.gurobi.com 
* [`rbison`](https://cran.r-project.org/web/packages/rbison): 查询USGS 'BISON数据库的R程序包，主要是北美物种分布数据 (https://bison.usgs.gov/#home)。
* [`rCAT`](https://cran.r-project.org/web/packages/rCAT): 物种保护等级的评估，用于编写红色名录，包括计算物种分布区大小，分布区范围等。 由Kew Gardens编写。
* [`rebird`](https://cran.r-project.org/web/packages/rebird): 鸟类分布记录eBird数据库的R程序包接口，可用多种方式查询数据库
* [`red`](https://cran.r-project.org/web/packages/red): 计算IUCN红色名录评估过程中的一些指数，如分布区大小，分布的国家，海拔范围， 生成kml文件等。该程序包是进行物种濒危等级评估人员的重要工具。
* [`redlistr`](https://cran.r-project.org/web/packages/redlistr): 用于IUCN红色名录评估过程中物种分布区变化，并推测未来分布区大小等
* [`rfishbase`](https://cran.r-project.org/web/packages/rfishbase): 查询http://www.fishbase.org 数据库中30000种鱼类的生物学、生态学、 形态学数据等
* [`rgbif`](https://cran.r-project.org/web/packages/rgbif): GBIF的R接口程序包， 可查询物种名，记录数量，数据的meta信息以及绘图等。 https://ropenscilabs.github.io/occurrence-manual/
* [`rinat`](https://cran.r-project.org/web/packages/rinat): 访问iNaturalist网站获取物种分布数据
* [`RInSp`](https://cran.r-project.org/web/packages/RInSp): 评估个体的生态位特化， 计算个体以及种群的生态位宽度 Arujo's E, IS, Petraitis's W, Roughgarden's WIC/TNW
* [`rioja`](https://cran.r-project.org/web/packages/rioja): 第四纪数据分析 including constrained clustering, WA, WAPLS, IKFA, MLRC and MAT transfer functions, and stratigraphic diagrams.
* [`rredlist`](https://cran.r-project.org/web/packages/rredlist): 查询 IUCN 红色名录数据库 http://apiv3.iucnredlist.org/api/v3/docs
* [`rvertnet`](https://cran.r-project.org/web/packages/rvertnet): 获取http://vertnet.org/数据库中脊椎动物数据， 可以按照物种和地点查询
* [`sads`](https://cran.r-project.org/web/packages/sads): 物种多度分布的极大似然模型
* [`sdm`](https://cran.r-project.org/web/packages/sdm): 生态学家Miguel Araujo研究组的程序包。该程序包的特点是: 面向对象，分析可重复，可编写扩展组件。
* [`SDMPlay`](https://cran.r-project.org/web/packages/SDMPlay): 主要用于生态位模型的展示与教学，包含两种模型BRT (Boosted Regression Trees) and MaxEnt (Maximum Entropy) ，同时提供AUC曲线等， 可评估模型的准确性。 
* [`sdmpredictors`](https://cran.r-project.org/web/packages/sdmpredictors): 下载物种分布模型的数据， 包括古气候和预测的未来气候数据
* [`SDMTools`](https://cran.r-project.org/web/packages/SDMTools): 澳大利亚人开发的程序包，用于物种分布区模型的评估、可视化与比较分析等
* [`sdmvspecies`](https://cran.r-project.org/web/packages/sdmvspecies): 为物种分布区模型生成虚拟物种 
* [`SiMRiv`](https://cran.r-project.org/web/packages/SiMRiv): 模拟(动物)个体的运动
* [`spacodiR`](https://cran.r-project.org/web/packages/spacodiR): 群落多样性的空间及系统发育分析 
* [`SPECIES`](https://cran.r-project.org/web/packages/SPECIES): 物种丰富度模型的拟合
* [`SPEDInstabR`](https://cran.r-project.org/web/packages/SPEDInstabR): 分析ModestR软件给出的物种潜在分布区，确定影响物种分布的主要因素等
* [`sperich`](https://cran.r-project.org/web/packages/sperich): 估计物种分布区范围，并计算生物多样性热点地区等
* [`spocc`](https://cran.r-project.org/web/packages/spocc): 可查询各大物种分布记录的数据库， 包括 Global Biodiversity Information Facility ('GBIF'), 'USGSs' Biodiversity Information Serving Our Nation ('BISON'), 'iNaturalist', Berkeley 'Ecoinformatics' Engine, 'eBird', 'AntWeb', Integrated Digitized 'Biocollections' ('iDigBio'), 'VertNet', Ocean 'Biogeographic' Information System ('OBIS'), and Atlas of Living Australia ('ALA'). 
* [`spThin`](https://cran.r-project.org/web/packages/spThin): 基于空间分布，筛选物种分布记录 (Robert P. Anderson 组)
* [`SSDM`](https://cran.r-project.org/web/packages/SSDM): Stacked Species Distribution Modelling， 基于Shiny界面的物种生态位模型预测。 该程序包能一次预测多个物种，并且有良好的界面支持。
* [`subniche`](https://cran.r-project.org/web/packages/subniche): 群落中生态位变化的补偿指数 Complementary indexes calculation to the Outlying Mean Index analysis to explore niche shift of a community and biological constraint within an Euclidean space, with graphical displays.
* [`Traitspace`](https://cran.r-project.org/web/packages/Traitspace): Laughlin研究组开发的程序包，可基于分层贝叶斯模型，用性状数据等估计物种在群落中出现的多度。
* [`untb`](https://cran.r-project.org/web/packages/untb): 模拟中性理论中的Ecological Drift
* [`usdm`](https://cran.r-project.org/web/packages/usdm): 物种分布模型中的不确定性分析
* [`vegdata`](https://cran.r-project.org/web/packages/vegdata): 从 http://www.synbiosys.alterra.nl/turboveg/ 和 http://www.vegetweb.de 两大植被网站下载数据，并提供植物名称处理的相关函数。
* [`velociraptr`](https://cran.r-project.org/web/packages/velociraptr): 古生物学数据下载、清洗、剔除和分析。
* [`wallace`](https://cran.r-project.org/web/packages/wallace): 物种分布区模型预测，使用Shiny GUI，用户可自己开发分析组件。 具备完成的分析流程，另可下载相应代码 ( https`](https://wallaceecomod.github.io/ )。
* [`zetadiv`](https://cran.r-project.org/web/packages/zetadiv): 计算zeta-diversity和物种组成变化
* [`zoon`](https://cran.r-project.org/web/packages/zoon): 可重复性，可分享的物种分布区预测流程

