# TIF-Seq
Transcript isoform sequencing (TIF-Seq)通过选择性同时测序5'和3'端，实现全长转录本的测序。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/963ab287-8982-4056-a520-8f91fb3d5bfb)

# 建库步骤
1. 通过用寡核苷酸取代5'帽来选择带帽的mRNA分子。为了达到这个结果，5'-磷酸基团从非帽盖rna中去除，
以区分它们与它们的帽盖rna。通过烟草酸性焦磷酸酶(TAP)处理去除帽，暴露5'-磷酸基团与寡核苷酸连接。
2. 将mrna分离到2个不同的管中并进行反转录以生成全长cDNA (flcDNA)。将每个试管中的flcDNA退火为条形
码的5'-生物素化引物和3'引物。引物包含每个试管独特的条形码序列，作为防止嵌合片段和分子间连接的控制机制。
3. 两根管结合，用NotI酶酶切产生粘端，并结扎形成环状双链cDNA，随后片段化。
4. 含有生物素化的3'和5'端片段用链霉亲和素分离。
5. 在纯化的cDNA片段的3′和5′端添加多路条形码，建立cDNA文库用于测序。

# Pros
1. 可以同时鉴定一个转录本的5'和3'端。
2. 嵌合体对照的barcode可以去除cDNA片段之间的连接。

# Cons
1. 样本需要具备大量的全长的RNA
2. 使用NotI酶引入粘性末端只适用于AT富集的基因组，类似酵母。
3. 对短片段和有偏差，因为短片段环化效率低。

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/tif-seq.html

Vicent Pelechano, Wu Wei, and Lars M. Steinmetz, “Extensive Transcriptional Heterogeneity Revealed by Isoform Profiling,” Nature 497, no. 7447 (May 2, 2013): 127–131, doi:10.1038/nature12121
        
        
        
        
