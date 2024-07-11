数据集：

[Store Sales - Time Series Forecasting](https://cloud.tencent.com/developer/article/2384397)

[Google Stock Price](https://www.kaggle.com/datasets/henryshan/google-stock-price)

[UCI:UCI ElectricityLoadDiagrams20112014](https://archive.ics.uci.edu/ml/machine-learning-databases/00321/LD2011_2014.txt.zip)

reference:
> [使用Transformer 模型进行时间序列预测](https://cloud.tencent.com/developer/article/2384397)

> [Kaggle实战：Store Sales - Time Series Forecasting](https://blog.csdn.net/weixin_43907802/article/details/122798776)

> [时序预测Time Series Forecasting:实体店销售](https://www.cnblogs.com/March7th/p/17289259.html)

---

对于Store Sales - Time Series Forecasting

比赛使用的评估指标是均方根误差（RMSLE）。（取对数意味着预测大的销售数字和小的销售数字的误差将更均匀地影响结果）

目标：预测未来16天每个产品、每个商店的销售情况。

---
VAR、ARDL:传统统计模型时间序列分析 

var文件里有统计检验分析 如协整检验

---
Temporal fusion transformer(TFT):参数量巨大的模型，跑通了但是没跑完,有模板
> [基于深度学习的时间序列预测:Temporal Fusion Transformer](https://blog.csdn.net/wjjc1017/article/details/135913845)

---
TCN：时域卷积网络(Temporal Convolutional Network)跑通了效果还行
> [PyTorch实现TCN时间卷积网络进行时间序列预测](https://blog.csdn.net/java1314777/article/details/134687303)

---
Crossformer：(还没跑)
> [时间序列预测实战Crossformer](https://blog.csdn.net/java1314777/article/details/134670578)
> [github](https://github.com/Thinklab-SJTU/Crossformer)

---
SegRNN：(还没跑)
> [SegRNN: Segment Recurrent Neural Network for Long-Term Time Series Forecasting](https://paperswithcode.com/paper/segrnn-segment-recurrent-neural-network-for)
> [github](https://github.com/lss-1138/SegRNN)
---
detrend：时间序列去趋势，傅里叶时间序列去噪

---
optuna：超参数调参

SHAP：模型无关的可解释性方法（还没看也没具体应用）
