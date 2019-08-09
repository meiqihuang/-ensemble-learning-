# 集成学习算法梳理（ensemble-learning）
## 1 Task1 随机森林算法梳理
见Task1 随机森林算法梳理.docx

## 2 Task2 GBDT
### 2.1 GBDT算法原理
GBDT 的全称是 Gradient Boosting Decision Tree，梯度提升决策树。基于梯度提升算法的学习器叫做 GBM(Gradient Boosting Machine)。理论上，GBM 可以选择各种不同的学习算法作为基学习器。GBDT 实际上是 GBM 的一种情况。

GBDT采用的是加法模型与前向分布算法。GBDT与Adboost最主要的区别在于两者如何识别模型的问题。Adaboost用错分数据点来识别问题，通过调整错分数据点的权重来改进模型。GBDT通过负梯度来识别问题，通过计算负梯度来改进模型。

下面主要对回归问题的提升树进行说明，依然采用前向分步算法，过程如下：
![前向分步算法](https://github.com/meiqihuang/-ensemble-learning-/blob/master/%E5%89%8D%E5%90%91%E5%88%86%E6%AD%A5%E7%AE%97%E6%B3%95.png)
