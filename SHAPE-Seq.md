# SHAPE-Seq
SHAPE-Seq 联合 2′-hydroxyl acylation analyzed by primer extension (SHAPE) 试剂和多重标记的双端技术。
SHAPE-Seq 可以提供RNA的二级结构信息。 

# 建库步骤
1. 特异的barcode首先连接到RNA的3'端。允许RNA在体外的条件下折叠。
2. 使用SHAPE试剂处理barcode和折叠的 RNA。该试剂是1-methyl-7-nitroisatoic anhydride (1M7)，它能屏蔽掉反转录。
3. RNA反转录成cDNA。
4. 深度测序cDNA可以获取1M7占据的位置的单碱基水平信息。
5. 根据以上信息推理出RNA的二级结构。

# Pros
1. 提供RNA的结构信息。
2. barcode可以标记不同的RNA。
3. RNA上的单碱基突变可以被检测到。
4. 可以替代质谱，核磁共振和晶体学。

# Cons
1. 需要正对照和负对照。
2. 需要提前构建RNA折叠的环境
3. 体外(in vitro)的折叠可能不会反应体内(in vivo)的折叠

# 参考文献
Julius B. Lucks et al., “Multiplexed RNA Structure Characterization with Selective 2′-hydroxyl Acylation Analyzed by Primer Extension Sequencing (SHAPE-Seq),” Proceedings of the National Academy of Sciences 108, no. 27 (July 5, 2011): 11063–11068, doi:10.1073/pnas.1106501108

https://www.illumina.com/science/sequencing-method-explorer/kits-and-arrays/shape-seq.html


