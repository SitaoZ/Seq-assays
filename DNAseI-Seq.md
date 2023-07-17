# DNAseI-Seq
DNase I 印迹最早发布月1978年，早于sanger测序和高通量测序。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/8f111098-6001-4c5c-bbf3-f919da207ce0)

# 建库方法
1. DNA和蛋白复合体使用DNase I处理。或者在处理之前使用紫外交联处理，固定DNA-蛋白质的结合
2. 若序列被蛋白质绑定，DNase I酶就无法降解该序列。
3. DNA提取，建库测序。

# Pros
1. 能检测染色质的开放性。
2. 无需事先知道序列和绑定蛋白。
3. 和FAIRE-Seq相比，DNaseI-Seq在启动子区域有更好的敏感性。

# Cons
1. DNase I是序列特异性的，且对位置高敏，因此不可能适用于全部基因组。
2. 多步纯化会导致DNA丢失，限制敏感性。
3. DNase I与ChIP数据的整合对于识别和区分相似的蛋白质结合位点是必要的

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/dnase-seq-dnasel-seq.html
Jay R. Hesselberth et al., “Global Mapping of protein-DNA Interactions in Vivo by Digital Genomic Footprinting,” Nature Methods 6, no. 4 (April 2009): 283–289, doi:10.1038/nmeth.1313
