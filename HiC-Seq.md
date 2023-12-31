# HiC-Seq

Hi-C也叫3C-Seq和Capture-C，是用来分析染色质相互作用的技术。Capture-C在3C方法中增加了一个额外的生物素化片段的磁珠下拉。
对Capture-C方法进行了新的改进(NG Capture-C)。Hi-C方法将3C-Seq扩展到 绘制全基因组染色质接触图谱; 它也被应用于研究原位染色质相互作用。

在这种方法中，dna -蛋白质复合物与甲醛交联。样品被切碎，DNA被提取、连接，并用限制性内切酶消化。产生的DNA片段被pcr扩增并测序。深度测序提供了结扎片段的碱基对分辨率。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/93d550cd-d861-4005-b22e-f2d2eeb5db55)


# Pros
1. 能检测到长距离的DNA的相互作用
2. 高通量

# Cons
1. 检测结果可能是随机的染色体碰撞。
2. 实际上只有不到1%的DNA片段产生链接产物。
3. 因为方法复杂，需要大量的初始材料。


# Terminology
<img src="https://github.com/SitaoZ/Seq-assays/assets/29169319/aa6efb1b-e776-4db8-ac76-dc6dd0c9b535" width="400" height="400">

1. 细胞核(nucleus)
真核生物中最大的细胞器，是细胞遗传和代谢控制中心。
核膜(nuclear envelope): 用来包裹染色质，控制物质进出  
核纤层(nuclear lamina): 位于核膜的内表面的纤维网络，支持核膜，锚定染色质，与核骨架相连，参与细胞周期解离和重建  
核仁(nucleolus): 主要存储合成 rRNA，存储装配核糖体  

2. 染色质疆域(chromosome territory, CT)
<img src="https://github.com/SitaoZ/Seq-assays/assets/29169319/693e9ab8-d73f-4674-8e8a-98ad781a9e3b" width="400" height="400">

染色质在细胞核内的分布不是随机的，各染色体占据不同的空间。
- 相对位置不变，染色体相对位置不变持续到有丝分裂起始。体积大且基因数目少的染色体位于核外围，体积小且基因数目多的染色体靠近核中心
- 染色质的位置因细胞类型的不同而产生相应的变化。如X染色体在肝脏细胞中更频繁地定位中外围

3. 染色质区室(A/B compartments)
<img src="https://github.com/SitaoZ/Seq-assays/assets/29169319/f96a90f9-75ba-4049-a709-ee500e77d223" width="400" height="200">

基因组被分成A/B两个区室，区室内部互作多，区室间互作少。
- A compartments
  开放的染色质，表达活跃，基因丰富，具有较高的GC含量，包含用于主动转录的组蛋白标记，通常位于细胞核的内部。
- B compartments
  关闭的染色质，表达不活跃，基因缺乏，结构紧凑，含有基因沉默的组蛋白标志物，位于核外围。主要由LAD组成，包含晚期复制起点。
- 在生信分析中，通过计算染色体内部互作的相关性来区分不同区室

4. 拓扑结构(topologically associating domains, TAD)
<img src="https://github.com/SitaoZ/Seq-assays/assets/29169319/4d30038e-0acb-4e79-9c3d-bdb6d310cf12" width="500" height="500">

在染色质区室中，存在互作频繁的基因组区域，称为拓扑结构域，TAD。
这些区域在不同物种和不同细胞中很保守，并且高度富集CTCF和粘连蛋白。
通过计算基因互作矩阵，我们会得到类似上图的大三角形，可以看到上面有几个深红色的三角，代表内部高度互作区域。一般是400-800kb长度。
TAD可以进一步细分为subTAD,大小约100kb, subTAD之间的边界在不同细胞的组织间具有差异性，与细胞特异的增强子-启动子互作有关。

5. 层关联域(Lamina accociating domains, LAD)
![btmgmn81ga](https://github.com/SitaoZ/Seq-assays/assets/29169319/1d9ff268-fb68-42c4-9a46-1e980842d146)

LAD是多细胞动物基因组中的异染色质结构域。在哺乳动物中，LAD的长度约为10kb-10Mb，覆盖30-40%的基因组。LAD主要由转录沉默染色质组成，富含H3K9me2、H3K9me3以及H3K27me3等
组蛋白修饰，主流观点认为LAD是一种染色质抑制状态。
- 结构性LAD(constitutive LAD, cLAD): 富含AT区域的异染色质区域，靠近核纤层，对染色体之间的结构形成至关重要
- 偶发性LAD(facultative LAD, fLAD): 具有不同的核纤层的相互作用，在不同细胞中抑制或者激活不同的基因，从而导致细胞类型

6. 核仁关联域(Nucleolar associating domains, NAD)
![ney9avuy8p](https://github.com/SitaoZ/Seq-assays/assets/29169319/9393790f-87d2-498e-ade2-14b8db9edff2)

NAD占基因组的4%，几乎具有与LAD相同的所有物理特征，通过对LAD和NAD的序列分析发现，某些区域可能在核纤层和核仁之间切换  

7. 染色质环(Chromatin loop)
<img src="https://github.com/SitaoZ/Seq-assays/assets/29169319/9145f63a-bce2-427d-a73f-c669eb9f24f5" width="600" height="400">

染色质子在空间中形成环状结构，因此相距很远的染色质区域可以在三维空间中聚在一起。
据推测大约50%的人类基因通过染色质环化的过程参与长距离的染色质互作。这种结构可以使线性距离很远的元件得以相遇，以此来完成调控作用。如空间上启动子和增强子结合激活转录。

# software
1. HiCExploer
基于Python的分析软件，接触矩阵获取，QC，标准化，TAD calling, Loop calling, 差异分析，可视化，格式转换等。
2. Juicebox
可以web浏览器上展示HiC数据，允许用户交互式地浏览、比较和分享。
3. TADCompare
基于R的TAD差异分析软件。
4. PASTIS
染色体3D结构推断软件。

# HiC辅助组装
HiC数据的互作在染色体内互作富集，互作随着距离衰减，因此在基因组组装中可以利用HiC数据的特征将contigs/scaffords挂载到pseudomolecules水平。
## 辅助组装软件
- 3D-DNA + Juicebox
```bash
# step 1 软件安装
git clone https://github.com/aidenlab/juicer.git
git clone https://github.com/aidenlab/3d-dna.git

# step 2
#对需要挂载的基因组建索引
bwa index xxx.fa
#根据基因组构建创建酶切位点文件
python generate_site_positions.py DpnII genome xxx.fa
#获取每条contig长度
awk 'BEGIN{OFS="\t"}{print $1, $NF}' genome_DpnII.txt > genome.chrom.sizes
#运行Juicer
sh /juicer.sh

# step 3
# Juicebox纠错

# step 4
sh run-asm-pipeline-post-review.sh 
```
- ALLHiC
[allhic-tutorial](https://github.com/tangerzhang/ALLHiC/wiki)

# Reference

Doğan, E.S., Liu, C. Three-dimensional chromatin packing and positioning of plant genomes. Nature Plants 4, 521–529 (2018). https://doi.org/10.1038/s41477-018-0199-5    
Krijger, P., de Laat, W. Regulation of disease-associated gene expression in the 3D genome. Nat Rev Mol Cell Biol 17, 771–782 (2016). https://doi.org/10.1038/nrm.2016.138   
Matharu, N., & Ahituv, N. (2015). Minor Loops in Major Folds: Enhancer-Promoter Looping, Chromatin Restructuring, and Their Association with Transcriptional Regulation and Disease. PLoS genetics, 11(12), e1005640. https://doi.org/10.1371/journal.pgen.1005640   
Erez Lieberman-Aiden et al., “Comprehensive Mapping of Long-Range Interactions Reveals Folding Principles of the Human Genome,” Science 326, no. 5950 (October 9, 2009): 289–293, doi:10.1126/science.1181369   
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/hi-c-3c-seq-capture-c.html  
        
        
        
        
        
        
        
        
        
        
