## RIP-Seq

![屏幕快照 2024-06-05 上午9 15 58](https://github.com/SitaoZ/Seq-assays/assets/29169319/dcf394b0-dfe3-451a-a3b1-02eb478fa278)


RNA Immunoprecipitation Sequencing (RIP-seq)以RNA免疫共沉淀（RIP）为基础，采用特异抗体对RNA结合蛋白或者特殊修饰的RNA进行免疫共沉淀后，分离RNA，通过Illumina测序，在全转录组范围内研究被特定蛋白特异结合的RNA区域或种类。

## 建库步骤
1.紫外交联，细胞裂解
2.提取染色质，随机打断
3.磁珠、抗体免疫共沉淀
4.RNA分离与纯化
5.文库构建，根据分析的RNA的类型的不同(mRNA,lncRNA, circRNA, small RNA)，可以分成多种文库



## 常见问题
Input对照组的设定：RNA片段化后，在进行免疫沉淀前，需要取一部分做Input对照（不进行免疫沉淀过程）。因此，Input和IP两个样本在前期检测、建库、测序都是平行进行的。  
Input对照组的作用：通过Input对照排除背景噪音（非特异性结合所造成的假阳性Peaks）， 验证RNA断裂的效果和整个实验中IP效果，所以Input 对照是IP-seq实验必不可少的步骤。
## 参考文献
RIP-Seq: Genome-wide identification of polycomb-associated RNAs by RIP-seq
