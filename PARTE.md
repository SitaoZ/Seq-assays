# PARTE
PARTE-seq (Parallel Analysis of RNA structures with Temperature Elevation)RNA结构与温度的关系测序。

# 建库步骤
该方法原先是在哺乳动物中开发的，所以原始的温度是37摄氏度。
1. RNA提取，包括复杂的RNA二级结构，和蛋白结合的RNA。
2. 37摄氏度温度Rnase V1处理, 能保持RNA中的双链结构，该酶处理后的样本进行ssRNA测序。
3. 经过上述Rnase V1处理过的的RNA，再进行 Rnase1处理，降解RNA，指只保留本蛋白结合的RNA,RBP或者其他蛋白，纯化RNA进行测序。
4. 另一个温度的处理，55摄氏度，重复上述步骤。

# 参考文献

Yue Wan et al., “Genome-wide Measurement of RNA Folding Energies,” Molecular Cell 48, no. 2 (October 26, 2012): 169–181, doi:10.1016/j.molcel.2012.08.008  
