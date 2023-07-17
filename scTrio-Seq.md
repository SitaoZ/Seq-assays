# scTrio-Seq
single-cell triple omics sequencing(scTrio-Seq)，scTrio-Seq可以同时分析单个哺乳动物细胞的基因组CNVs、DNA甲基化组和转录组。
这种方法是对以前的方法(如scMT-seq)的扩展。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/653db4b3-98e9-4c31-9a09-c158d6e63526)

# 建库步骤
1. 单细胞悬浮液制备，分选单细胞
2. 细胞质和细胞核的分离，实现了物理上DNA和RNA的分离
3. 对于RNA使用scRNA-Seq的建库方式，[scRNA-Seq建库原理](https://teichlab.github.io/scg_lib_structs/methods_html/tang2009.html)。
4. 对于DNA使用scRRBS建库[scRRBS建库原理](https://teichlab.github.io/scg_lib_structs/methods_html/scRRBS.html)。

# Pros
1. 能准确分析转录组，基因组和DNA甲基化，以及他们相互之间的作用。
2. 使用scRRBS的数据来准确获取CNVs

# Cons
1. 和scMT-Seq相比，转录本的覆盖度比较低
2. 转录组的3'端结果存在偏差

# 注意
1. scRRBS, single-cell reduced representation bisulfite sequencing, 重亚硫酸盐处理测序，将没有甲基化的胞嘧啶C转化成U，该过程叫做 Bisulfite converstion
2. scMT-Seq, 也是物理分割细胞质和细胞核进行测序。细胞质中的mRNA进行SMRT2-Seq测序。细胞核中的基因组机型scRRBS测序

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer.html
https://teichlab.github.io/scg_lib_structs/methods_html/scTrio-seq.html
