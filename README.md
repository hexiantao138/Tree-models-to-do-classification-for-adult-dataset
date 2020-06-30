# 基于机器学习模型的成人年薪预测
* 数据集与具体描述可以在此下载: http://archive.ics.uci.edu/ml/datasets/Adult
* 原始数据表格如下:
![](/raw_data.png)
## 数据预处理: 
* 删除Null值。 
* 去除重复行。
* 将分类型特征值进行one-hot编码。 
* 将年薪分类<=50k标注为0，>50k标注为1。
* 数据预处理之后的表格如下:
![](/data_preprocess.png)
## 数据分析与可视化 
* 画热图来量化各特征间的相关性
![](/heatmap_of_variable_correlation.png)
* 画箱形图检验各特征异常值以及各特征对预测结果的影响
![](/Boxplots%20for%20predictors%20versus%20target%20variable.png)
* 用pairplot来展现变量间的线性关系，并用散点图呈现
![](/pairplot%20of%20adult.png)
## 构建机器学习模型 
* 使用scikit-learn包中的决策树与随机森林模型。
* 对测试集进行上述步骤预处理，根据学习的模型进行年薪预测。
