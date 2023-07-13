# GRO-Seq
GRO-Seq (Global nuclear Run-On sequencing)是一种专门测量新生RNA的方法。可用于enhancer RNA (eRNA)的鉴定。
# 建库步骤
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/a5a1f66d-13f8-4bf6-afb7-c83c78969ebd)
1. 使用冷PBS溶液对细胞进行清洗，迅速冷冻细胞，使细胞核内RNA聚合酶形成的复合物停滞在转录的状态。
2. 提取细胞的细胞核，并加入Run-on缓冲液，让细胞核内的转录复合物重新恢复到转录状态。在加入Run-on缓冲液的同时掺入Br-UTP（溴尿嘧啶），BrU可以代替正常的尿嘧啶参与到转录中去。（溴尿嘧啶其实就是尿嘧啶5'上的氢被溴替代产生的一种示踪剂，因为溴比较重，可以通过离心分离出来）。
3. 让转录进行一段时间，新生的RNA上都具有溴尿嘧啶的标记，如果是从转录起始位点开始进行的转录，它的5'端上还会具有帽结构（具体见CAGE-seq一文）。
4. 提取新生的RNA，并用带有BrU抗体的磁珠将这些新生的RNA都富集出来。
5. 再次纯化，去除帽结构，修复末端，连接接头。
6. 反转录产生cDNA，上机测序。
# 几点说明
## Pros (优点)
1. 能够找到RNA聚合酶绑定的转录位点
2. 鉴定转录的相对活性
3. 检测正义链和反义链的转录本
4. 全基因组层面检测转录活性位点
5. 不需要事先知道转录起始位点的信息
6. 提供增强子相关RNA和启动子相关RNA的信息


## Cons (缺点)
1. 因为需要在核苷酸标记下进行复苏，GRO-Seq建库对条件要求比较严格。
2. 在制备过程中会引入伪序列。
3. 在run-on 步骤中，可能会引入新的转录起始位点，因为aTSS的存在。
4. 物理障碍可能会阻断RNA聚合酶。
5. 分辨率只有30-100 nt。
6. 至少需要18-nt的初生链。
7. GRO-seq对样本数量有很高的要求，因为它的测序完全依赖于新生的RNA，单细胞的GRO-seq基本上是不可行的，因为很难保证每个细胞在冷冻处理后都可以恢复转录。
8. 如果你处理过GRO-seq数据，你会发现它的信号比一般的RNA-seq要强很多，这也可能是样本量导致的。
9. 有条件的实验室可以把提取好的细胞核冷冻后送给公司测序，不过一般来说还是送活细胞和培养基吧.....
# 参考文献
Leighton J. Core, Joshua J. Waterfall, and John T. Lis, “Nascent RNA Sequencing Reveals Widespread Pausing and Divergent Initiation at Human Promoters,” Science 322, no. 5909 (December 19, 2008): 1845–1848, doi:10.1126/science.1162228
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/gro-seq-bric-seq-bru-seq-bruchase-seq.html
https://zhuanlan.zhihu.com/p/52114556
https://liorpachter.wordpress.com/seq/
        
        
        
        
        
