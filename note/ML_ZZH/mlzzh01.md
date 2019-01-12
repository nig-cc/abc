# 绪论
## 什么是机器学习

我们根据过去的经验来判断明天的天气，根据购买经验来挑选一个好瓜，`通过对以往经验的利用，就能对新的情况做出有效的决策`。机器学习正是这样的一门学科，人的“经验”对应计算机中的“数据”，让计算机来学习这些经验数据，生成一个算法模型，在面对新的情况中，计算机便能作出有效的判断，这便是机器学习。

## 基本术语

假设我们收集了一批西瓜的数据,例如:

    (色泽=青绿;根蒂=蜷缩;敲声=浊响),
    (色泽=乌黑;根蒂=稍蜷;敲声=沉闷),
    (色泽=浅自;根蒂=硬挺;敲声=清脆)
    ……

每对括号内是一个西瓜的记录,则有如下定义:

- 这组记录的集合:**数据集(data set)**
- 其中每一条记录是关于一个事件或对象的描述:**一个示例(instance)或样本(sample)**
- 反映事物或对象在某方面的表现或性质的事项(如色泽或敲声):**特征(feature)或属性(attribute)**
- 属性上的取值:**属性值(attribute value)**
- 属性张成的空间:**属性空间 (attribute space)、 样本空间 (samp1e space)或输入空间(input space)**

`如我们把"色泽" "根蒂" "敲声"作为三个坐标轴，则它们张成一个用于描述西瓜的三维空间，每个西瓜都可在这个空间中找到自己的坐标位置`

- 由于空间中的每个点对应一个坐标向量，因此一个示例也称为**一个特征向量(feature vector)**
- 一个样本的特征数:**维数(dimensionality)**
- 从数据中学得模型的过程:**学习(learning)或训练(training)**
- 训练过程中使用的数据:**训练数据(training data)**
- 其中每一个样本:**训练样本(training sample)**
- 训练样本组成的集合:**训练集(training set)**
- 学得模型对应了关于数据的某种潜在的规律:**假设(hypothesis)**
- 这种潜在的规律自身:**真相(ground-truth)**

`学习的过程就是为了找出或逼近真相`

- 关于示例结果的信息:**标签(label)**
- 拥有了标签信息的示例:**样例(example)**
- 所有标签的集合:**标签空间(label space)或(output space)**
- 若欲预测的是离散值，此类学习任务:**分类(classification)**
- 欲预测的是连续值，此类学习任务:**回归(regression)**
- 只涉及两个类别的分类任务:**二分类(binary classification)**
- 通常称其中一个类为**正类 (positive class)**，另一个类为**反类 (negative class)**
- 涉及多个类别的分类任务:**多分类(multi-class classification)**

一般地，预测任务是希望通过对训练集进行学习，建立一个从输入空间到输出空间的映射

- 学得模型后，使用其进行预测的过程:**测试(testing)**
- 被预测的样本:**测试样本(testing sample)**
- 学得模型适用于新样本的能力:**泛化(generalization)能力**
- 通常假设样本空间中全体样本服从一个未知分布，我们获取的样本都是独立地从这个分布上采样获得的:**独立同分布(independent and identically distributed)**

## 
