# Frag-Seq
Fragmentation sequencing (FRAG-Seq，片段化测序法) 是一种用来捕获RNA二级结构的测序方法。在该方法中,RNA首先被核酸酶P1酶解，然后反转录成cDNA. 
高通量测定cDNA能提供高分辨率的单链read，通过read比对回P1的剪切位点，可确定核酸酶P1剪切位点的结构。
![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/c49c2e57-8598-4437-af26-ac92e983fc77)

# 建库步骤
1. RNA提取， P1核酸内切酶处理，得到20–100-nt片段。
2. 在片段的5'-PO4和3'-OH端分别加上测序接头。
3. 通过逆转录和PCR扩增之后，构建Frag-Seq文库并对其进行深测序。
4. 为了保证文库片段均是由核酸酶P1剪切产生，需要设置两个对照组：一组RNA不使用核酸酶P1处理来估算由内源降解产生5'-PO4基团的片段数，另一组则多加了T4连接酶处理RNA，以此来计算不产生5'-PO4基团的片段数
5. 
# Pros:
1. P1 核酸内切酶。Nuclease P1 是一种单链特异性内切酶, 广泛应用于制药和食品工业领域，能水解核苷酸成5'-核苷酸单体，也能剪切掉双链核苷酸的单链区域。
2. 基于P1的特点可以研究RNA的二级结构，看RNA的双链形成的位置。
3. 和PARS-Seq技术相比，Frag-Seq的操作比较简单快速。
4. 通量高。
5. 可以替代质谱，核磁共振和晶体学。

# Cons:
1. 需要内源的对照。
2. 样本和对照之间可能存在污染。

# 参考文献
https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/frag-seq.html
https://news.sciencenet.cn/htmlpaper/20101291645135413857.shtm
