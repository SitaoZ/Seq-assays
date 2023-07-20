# oxBS-Seq
oxBS-Seq (Oxidative bisulfite sequencing) 氧化亚硫酸盐测序能区分5mC和fhmC。
在oxBS-Seq中，5hmC (5位羟甲基)氧化生成5fC (5为甲酰基)，5mC保持不变。
亚硫酸氢钠处理，5hmC转化成T。比较处理和未处理的样本就可以鉴定5mC的位点，达到碱基水平的分辨率。

![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/614f92b0-027c-49b8-b553-9bec39227c58)

# Pros
1. 全基因组水平的CpG和non-CpG的甲基化都能在碱基水平被全覆盖。
2. 5mC密集和低密集的重复区域被覆盖。
3. 方法清晰区分5mC和5hmC，准确识别5mC。

# Cons
1. 亚硫酸氢盐将未甲基化的胞嘧啶转化为胸腺嘧啶，降低了序列的复杂性，这使得序列比对变得困难。
2. 亚硫酸盐转化时，胞嘧啶C转化为胸腺嘧啶T的位点如果是SNP位点，那么该SNP信息将被遗漏。

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/oxbs-seq.html

Michael J. Booth et al., “Quantitative Sequencing of 5-Methylcytosine and 5-Hydroxymethylcytosine at Single-Base Resolution,” Science 336, no. 6083 (May 18, 2012): 934–937, doi:10.1126/science.1220671
        
        
        
        
        
        
