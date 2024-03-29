# MIMO - OFDM 实验

多入多出 正交频分复用

基于正交频分复用和多输入多输出的无限通信系统

## OFDM
使用离散傅里叶变换实现OFDM
实际应用采用快速傅里叶变换

## MIMO 

通过增加天线数量实现

利用空间资源换取频谱资源

## MIMO-OFDM系统模型

在典型的MIMO-OFDM系统模型中，发射端（N个发射天线）工作流程如下：
输入的数据符号流经串/并电路分成N个子符号流，
采用信道编码技术对每个符号流进行无失真压缩并加入冗余信息，
调制器对编码后的数据进行空时调制；
调制后的信号在IFFT电路中实现OFDM调制处理，完成将频域数据变换为时域数据的过程，
然后输出的每个OFDM符号前加一个循环前缀以减弱信道延迟扩展产生的影响，
每个时隙前加前缀用以定时，这些处理过的OFDM信号流相互平行地传输，
每一个信号流对应一个指定的发射天线，并经数模转换及射频模块处理后发射出去。
