# iCLIP-Seq

![屏幕快照 2024-06-05 上午9 42 24](https://github.com/SitaoZ/Seq-assays/assets/29169319/003bd41b-25fe-4d33-8fe0-dcfd64b6d854)



iCLIP-Seq (individual-nucleotide resolution cross-linking and immunoprecipitation) 
iCLIP绘制蛋白质-rna相互作用，其过程类似于HITS-CLIP和PAR-CLIP。这种方法包括在交联后消化蛋白质和用逆转录酶绘制交联位点的额外步骤。  
在iCLIP中，特异性交联rna-蛋白复合物被免疫沉淀。复合物用蛋白酶K处理，因为在结合位点交联的蛋白质仍然未被消化。在RT上，cDNA在结合位
点截短并循环。这些环状片段被线性化并进行pcr扩增。这些扩增片段的深度测序提供了蛋白质结合位点的核苷酸分辨率，eCLIP是对iCLIP的改进，
避免了循环cDNA以减少伪影。

# Pros  
1. 碱基水平的精度识别蛋白质结合位位点
2. 避免核酸酶的使用
3. 扩增会检测到稀有的互作
Nucleotide resolution of protein-binding sites
Avoids the use of nucleases
Amplification allows the detection of rare events

# Cons  
1. 非特异性抗体会沉淀非特异性复合物
2. 非线性PCR扩增可导致影响可重复性的偏差
3. 循环步骤中引入假阳性
4. 用于可视化紫外交联蛋白- rna复合物所需的放射性同位素仅标记5'端
5. 环化链接效率不够高

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer.html



