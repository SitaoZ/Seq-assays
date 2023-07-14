# Structure-Seq/DMS-Seq
DMS-Seq (dimethyl sulphate sequencing)，硫酸二甲酯测序法，该方法可以在体内和体外对RNA的结构实现单碱基精度的测序。
使用DMS化学修饰未配对的腺嘌呤(adenines)和胞嘧啶(cytosines),实现RNA二级结构的鉴定。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/3abba870-d6fd-41f3-a90e-4991640ee31f)


# 建库步骤
1. DMS处理样本，实现in vivo地标记RNA的二级结构。
2. RNA提取，poly(A)富集，使用DNase处理。
3. 使用随机的六聚体(hexamers)作为随机引物，启动反转录。
4. 反转录的第一链链接单链的DNA linker, 使用环化酶(CircLigase enzyme)进行自连环化。
5. PCR扩增DNA (PCR-amplified)。
6. 片段选择(size-selection)。
7. 测序。

# Pros
1. 全基因组实现单碱基精度的鉴定RNA结构
2. 体内(in vivo)，体外(in vitro)均适用。
3. DMS可以穿越细胞膜，能够用于体内的应用。
4. 一个RT引物合成可以检索成千上万个RNA结构的信息
5. 随机六聚物引物最大限度地减少了3'端偏差

# Cons
1. 在体内，RBP能够屏蔽DMS修饰。
2. 环化会导入而外的偏差。

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/structure-seq-dms-seq.html
Silvi Rouskin et al., “Genome-wide Probing of RNA Structure Reveals Active Unfolding of mRNA Structures in Vivo,” Nature advance online publication (December 15, 2013), doi:10.1038/nature12894
        
        
Yiliang Ding et al., “In Vivo Genome-wide Profiling of RNA Secondary Structure Reveals Novel Regulatory Features,” Nature advance online publication (November 24, 2013), doi:10.1038/nature12756
        
        
        
        
