## MNase-Seq

![image](https://github.com/SitaoZ/Seq-assays/assets/29169319/e937d3a4-0fce-4302-97c6-801919473cc5)
Micrococcal nuclease (MNase), 微球菌核酸酶, 一种来源于微球菌的核酸酶，能够切割DNA和RNA。
微球菌核酶首先在金黄色葡萄球菌(革兰氏阳性菌)中发现，它能将染色质降解成200bp左右的核小体单元。   
在MNase-Seq中，gDNA使用MNase处理，被染色质蛋白保护的序列不会被降解，然后提取被保护的DNA，建库测序。
所以MNase-Seq用来鉴定染色质开放区域。

## 优点
- 能定位核小体和DNA绑定蛋白
- 能鉴定~25bp左右的亚核小体结构
- 鉴定基因组中不同类型的调控蛋白
- 能覆盖基因组中大部分的调控位点

## 缺点
- MNase切割位点不能覆盖全基因组
- AT碱基依赖偏差
- 整合MNase与ChIP数据对于识别和区分相似的蛋白质结合位点是必要的

## 建库手册

[Mnase star protocols](https://star-protocols.cell.com/protocols/666)
