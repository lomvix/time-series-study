数据集：

[Store Sales - Time Series Forecasting](https://cloud.tencent.com/developer/article/2384397)

[Google Stock Price](https://www.kaggle.com/datasets/henryshan/google-stock-price)

[UCI:UCI ElectricityLoadDiagrams20112014](https://archive.ics.uci.edu/ml/machine-learning-databases/00321/LD2011_2014.txt.zip)

[IGBT Accelerated Aging Data Set - NASA](https://data.nasa.gov/download/7wwx-fk77/application%2Fzip)

reference:
> [使用Transformer 模型进行时间序列预测](https://cloud.tencent.com/developer/article/2384397)

> [Kaggle实战：Store Sales - Time Series Forecasting](https://blog.csdn.net/weixin_43907802/article/details/122798776)

> [时序预测Time Series Forecasting:实体店销售](https://www.cnblogs.com/March7th/p/17289259.html)

>[金融时间序列分析讲义](https://www.math.pku.edu.cn/teachers/lidf/course/fts/ftsnotes/html/_ftsnotes/index.html)

>[time series library](https://github.com/thuml/Time-Series-Library)

---

对于Store Sales - Time Series Forecasting

比赛使用的评估指标是均方根误差（RMSLE）。（取对数意味着预测大的销售数字和小的销售数字的误差将更均匀地影响结果）

目标：预测未来16天每个产品、每个商店的销售情况。

---

信号相关的模型与处理

FAN：傅里叶分析网络 (FAN)[https://github.com/YihongDong/FAN/tree/main]

LSM：Liquid State Machine (LSM)，脉冲神经网络变体

VAR、ARDL:传统统计模型时间序列分析 

var文件里有统计检验分析 如协整检验

detrend：时间序列去趋势，傅里叶时间序列去噪

VMD：变分模态分解,是一种用来分离非固定频率信号的方法。

wavelet denoise：时间序列小波降噪

---
LSTM: 里面有两个模板，后面一个模板相对简单理解

---
Temporal fusion transformer(TFT):参数量巨大的模型，跑通了但是没跑完,有模板
> [基于深度学习的时间序列预测:Temporal Fusion Transformer](https://blog.csdn.net/wjjc1017/article/details/135913845)

---
TCN：时域卷积网络(Temporal Convolutional Network)跑通了效果还行
> [PyTorch实现TCN时间卷积网络进行时间序列预测](https://blog.csdn.net/java1314777/article/details/134687303)
>
> [TCN](http://home.ustc.edu.cn/~liujunyan/blog/tcn/)

---
Crossformer：(还没跑)
> [时间序列预测实战Crossformer](https://blog.csdn.net/java1314777/article/details/134670578)

> [github](https://github.com/Thinklab-SJTU/Crossformer)

---
SegRNN：(还没跑)
> [SegRNN: Segment Recurrent Neural Network for Long-Term Time Series Forecasting](https://paperswithcode.com/paper/segrnn-segment-recurrent-neural-network-for)

> [github](https://github.com/lss-1138/SegRNN)
---
Mamba：
> [Mamba的架构及实现](https://mp.weixin.qq.com/s?__biz=MzI1MjQ2OTQ3Ng==&mid=2247630782&idx=1&sn=82a2d74642278e0fb03f0954a03b7692&chksm=e8d0e224b82c7033404262318f4c8a6f3f50db716d32dc6e4f3fb870bca2fe5b757f9d1940d7&scene=27)

Simba:

[github](https://github.com/badripatro/Simba)

paper:[SiMBA: Simplified Mamba-Based Architecture for Vision and Multivariate Time series](https://arxiv.org/abs/2403.15360)

---
iTransformer：[iTransformer深度解析：时序预测新SOTA](https://blog.csdn.net/qq_33431368/article/details/134543912?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522172111726316800188518259%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=172111726316800188518259&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_click~default-4-134543912-null-null.142^v100^pc_search_result_base3&utm_term=iTransformer&spm=1018.2226.3001.4187)

[github](https://github.com/lucidrains/iTransformer)

---
PatchTST:(跑通了)

[Transformer时间序列：PatchTST引领时间序列预测](https://blog.csdn.net/weixin_42010722/article/details/131430367)


---
optuna：超参数调参[使用optuna对模型的超参数进行自动优化](https://www.jianshu.com/p/2513dc63e0ba)



SHAP：模型无关的可解释性方法（还没看也没具体应用）


NeuralForecast：集成时间序列模型的库 [NeuralForecast](https://blog.csdn.net/FrankieHello/article/details/135190192?spm=1001.2101.3001.6650.3&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ECtr-3-135190192-blog-136980609.235%5Ev43%5Epc_blog_bottom_relevance_base5&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ECtr-3-135190192-blog-136980609.235%5Ev43%5Epc_blog_bottom_relevance_base5&utm_relevant_index=2)
