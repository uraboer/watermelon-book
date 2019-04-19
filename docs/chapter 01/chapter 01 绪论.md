# CH01 绪论

## 基本术语

- 数据集（data set）：这组记录的集合
- 示例（instance）/样本（sample）：关于一个事件或对象的描述
- 属性（attribute）/特征（feature）：反应事件或对象在某方面的表现或性质的事项
- 属性值（attribute value）：属性上的取值
- 属性空间（attribute space）/样本空间（sample space）/输入空间：属性张成的空间
- 特征向量（feature vector）：一个示例
- 维数（dimensionality）：每个示例由d个属性描述
- 训练数据（training data）：训练过程中使用的数据
- 训练样本（training sample）：训练过程中的每个样本
- 训练集（training set）：训练样本组成的集合
- 假设（hypothesis）：学得模型对应了关于数据的某种潜在的规律
- 分类（classification）：此类学习任务预测的是离散值
- 回归（regression）：此类学习任务预测的是连续值
- 二分类（binary classification）：只涉及两个类别的学习任务，正类（positive class），负类（negative class）
- 测试（testing）：学得模型后，使用其进行预测的过程
- 测试样本（testing sample）：被预测的样本
- 聚类（clustering）：将训练集中的数据分成若干组，每组为一个簇（cluster）
- 泛化（generalization）：学得模型适用于新样本的能力
- 独立同分布（independent and identically distributed）：或得的每个样本都是独立地从这个分布上采样获得的

## 假设空间

- 归纳（induction）：从特殊到一般的泛化过程，即从具体的事实归结出一般性规律
- 演绎（deduction）：从一般到特殊的特化过程，即从基础原理推演出具体状况
- 版本空间（verison space）：可能有多个假设与训练集一致，即存在着一个与训练集一致的假设集合

## 归纳偏好

- 归纳偏好：机器学习算法在学习过程中对某种类型假设的偏好

- 奥卡姆剃刀（Occam’s razor）：若有多个假设与观察一致，则选择最简单的那个

- NFL定理（No Free Lunch Theorem）：

  $$\begin{aligned}
  \sum_{f}E_{ote}(\mathfrak{L}_a\vert X,f) &= \sum_f\sum_h\sum_{x\in\mathcal{X}-X}P(x)\mathbb{I}(h(x)\neq f(x))P(h\vert X,\mathfrak{L}_a) \\
  &=\sum_{x\in\mathcal{X}-X}P(x) \sum_hP(h\vert X,\mathfrak{L}_a)\sum_f\mathbb{I}(h(x)\neq f(x)) \\
  &=\sum_{x\in\mathcal{X}-X}P(x) \sum_hP(h\vert X,\mathfrak{L}_a)\cfrac{1}{2}2^{\vert \mathcal{X} \vert} \\
  &=\cfrac{1}{2}2^{\vert \mathcal{X} \vert}\sum_{x\in\mathcal{X}-X}P(x) \sum_hP(h\vert X,\mathfrak{L}_a) \\
  &=2^{\vert \mathcal{X} \vert-1}\sum_{x\in\mathcal{X}-X}P(x) \cdot 1\\
  \end{aligned}$$

## 发展历程



## 应用现状

