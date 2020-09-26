# MY_AL_Learning
记录进组后的学习过程。

###### 2020/8/31
- 今日工作：搬电脑和书到实验室。
- 明日安排：
    1. 结合论文（主动学习算法研究进展 杨文柱，田潇潇，王思乐， 张锡忠）学习代码（[deep-active-learning](https://github.com/ej0cl6/deep-active-learning)）；
    2. 分析问题，找论文；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 做论文记录。

---
#### 2020/9计划
1. 9月30号做小组论文分享。
2. 针对研究问题和自己的猜想，至少实现三种猜想，对比分析。
    1. 学习deep-active-learning代码（一周：9/1-9/6）；
    2. 修改代码（两周：9/7-9/20）；
        1. 画图（uncertainty-query次数/score_acc-query次数）；
        2. 保存模型（暂定 N = 5 ）；
        3. 利用模型（预计至少设置45组实验）；
    3. 对比结果（一周：9/21-9/27）。
---

###### 2020/9/1
- 今日工作：
    1. 学习代码：看到模型训练部分；
    2. 矩阵论（网课）第一课时：矩阵论的三个理论问题；
    3. 机器学习（网课）第一章：机器学习的定义+分类；
    4. 分析问题，查论文；
- 明日安排：
    1. 学习代码；
    2. 看论文：[Learning Loss for Active Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9027824)；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 看Docker容器技术；
    
###### 2020/9/2
- 今日工作：
    1. 机器学习（网课）第二章的一半:单元线性回归：假设空间（Hypothesis Space）+损失函数（Cost Function）；
    2. 学习代码（看完随机采样RandomSampling）：准备数据+训练测试（query10次）；
    3. 看Docker容器技术（第二章）：Docker->用于打包的容器（集装箱），基本可运行在所有操作系统上。
    4. 矩阵论（网课）第二课时：线性代数复习；
    5. 论文：看了摘要+引言的部分。
- 明日安排：
    1. 改代码（基于不确定性采样），画图（uncertainty-query次数/score_acc-query次数）；
    2. 机器学习（网课）；
    3. 看Docker容器技术；
    4. 看论文：Learning Loss for Active Learning；
    5. 矩阵论（网课）；
    6. 统计学习方法（李航）。
    
###### 2020/9/3
- 今日工作：
    1. 改代码（基于最低置信度采样）:保存query次数+未标记样本的置信度+模型+accuracy；
    2. 机器学习（网课）第二章的剩余部分：学习的ML的第一个算法——梯度下降算法（Gradient descent algorithm）；
    3. Docker容器技术（第三章）：镜像；
    4. 矩阵论（网课）第三课时三分之一；
    5. 论文：看完引言+相关工作+方法介绍的前部分；
    6. 统计学习方法（李航）：3.3.1构造平衡kd树。
- 明日安排：
    1. 改代码（基于最低置信度采样）：N=2+保留最近的N个模型+越近权重越大。
    Q1：uncertainty-query次数（uncertainty是算所有未标记样本置信度的平均值吗？）
    Q2：权重如何分配。
    2. 看论文：Learning Loss for Active Learning；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。
    
###### 2020/9/4
- 今日工作：
    1. 改代码（基于最低置信度采样）：保存最近的N=2个模型。
    2. 机器学习（网课）第三章:现代回顾（矩阵乘法+逆+转置）；
    3. 论文：实验评估的一小部分；
    4. 统计学习方法（李航）：搜索kd树+朴素贝叶斯分类器；
    5. 矩阵论（网课）第三课时：向量组的极大线性无关组+秩。
- 明日安排：
    1. 改代码（基于最低置信度采样）：越近权重越大；
    2. 看论文：Learning Loss for Active Learning，查新论文；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。

###### 2020/9/5
- 今日工作：
    1. 改代码（基于最低置信度采样）：越近权重越大(N=2,3,4,5);
    2. 论文:实验评估——图像分类+目标检测；
    3. 机器学习（网课）第五章前半部分；
    4. 统计学习方法（李航）:朴素贝叶斯算法的基本原理——》后验概率最大化==期望风险最小化。  
- 明日安排：
    1. 改代码（基于最低置信度采样）：N=2+保留准确率最高的N个模型+准确率越高权重越大;
    画loss-query次数。
    2. 看论文：Learning Loss for Active Learning+Batch Active Learning With Two-Stage Sampling；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。

###### 2020/9/6
- 今日工作：
    1. 改代码（基于最低置信度采样）:
    a. 画多个log文件acc-query图。
    b. CIFAR-10数据集：N=2+保留最近的N个模型+越近权重越大。
    c. 保存准确率最高的N个模型, 准确率越高权重越大。
    换数据集（CIFAR-10/CIFAR-100），最后如果在声纹里面效果比较好就更好。
    2. 论文：
    a. 看完了Learning Loss for Active Learning；
    3. 机器学习（网课）第五章后半部分；
    4. 统计学习方法（李航）:第4章朴素贝叶斯算法的参数估计——极大似然估计+贝叶斯估计；
    5. 矩阵论（网课）第四课：线性空间和线性变换；
- 明日安排：
    1. 改代码（基于最低置信度采样）：改用GPU跑;
    画loss-query次数；
    对CIFAR10改变pool和query数量。
    2. 看论文：Batch Active Learning With Two-Stage Sampling；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。
    
###### 2020/9/7
- 今日工作：
    1. 论文：摘要；
    2. 代码：
    a. 跑MNIST和CIFAR10的Rescent+AccMax和AccMax+RescentMax;
    3. 统计学习方法（李航）:决策树前部分。
    4. 机器学习（吴恩达）:第七章逻辑回归，线性回归外加Sigmoid函数；
    5. 矩阵论（网课）第五课：1/3处；
- 明日安排：
    1. 看论文：Batch Active Learning With Two-Stage Sampling；
    2. 改代码（基于最低置信度采样）：改用GPU跑;
    画loss-query次数；
    对CIFAR10改变pool和query数量。
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。
    
###### 2020/9/8
请假
    
###### 2020/9/9
- 今日工作：
    1. 机器学习（网课）第八章正则化：防止过拟合；
    2. 统计学习方法（李航）：决策树的特征选择——信息增益（information gain）；
    3. 论文:引言；
    4. 矩阵论（网课）：第五课看完了；
- 明日安排：
    1. 构建新项目（AL_utilize_previous_models）；
    2. 看论文：Batch Active Learning With Two-Stage Sampling；
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）。
    
###### 2020/9/10
- 今日工作：
    1. 构建新项目（AL_utilize_previous_models 私有）
    a. 初始有标记样本池1000个样本+每次query100个样本；
    b. query策略更换为随机采样;
    2. 论文：相关工作。
- 明日安排：
    1. 看论文：Batch Active Learning With Two-Stage Sampling；
    2. AL_utilize_previous_models：更换模型（ResNet,VGG,AlexNet,LeNet）
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）；
    6. Pytorch教程。
###### 2020/9/11
- 今日工作：
    1. 论文:BATCH SAMPLING WITH BOUNDARY ANNOTATION第一小部分；
    2. 项目AL_utilize_previous_models
    a. 更换模型:ResNet-18;
    3. 机器学习（网课）第9章:神经网络学习 看了一半；
    4. A Survey of Deep Active Learning看了一点；
    5. 统计学习方法（李航）:信息增益比;
    6. Pytorch教程:单车预测。
    
###### 2020/9/12
- 今日工作：
    1. 论文：initial seed sample based on clustering+依据多条规则批量采样；
    2. AL_utilize_previous_models:
    a. 跑MNIST/CIFAR10+ResNet-18+随机采样;
    b. 跑CIFAR10+ResNet-18+最低置信度；
    3. 机器学习（网课）第9章:神经网络学习 看完了；
    4. 统计学习方法（李航）:决策树的生成（ID3，C4.5）;
- 明日安排：
    1. 看论文：Batch Active Learning With Two-Stage Sampling；
    2. 跑代码：
    MNIST+ResNet-18+最低置信度；
    增加其他网络。
    3. 机器学习（网课）；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）；
    6. Pytorch教程。
    
###### 2020/9/13
- 今日工作：
    1. 论文:实验的前半部分；
    2. 统计学习方法（李航）：决策树的剪枝（基于损失计算），CART生成（划分标准->回归树：平方误差最小化；分类树：基尼系数最小化）；
    3. 改项目名：AL_UPM;
    4. 机器学习（网课）:反向传播+梯度检测;
    
- 明日安排：
    1. 跑代码：
    CIFAR10+ResNet-18+N-5_Rescent_RescentMax重跑3次
    CIFAR10+ResNet-18+边缘采样；
    2. 画图：Average Accuracy-Number of Labeled Examples.+重复实验5次。
    3. 看论文：
    Batch Active Learning With Two-Stage Sampling；
    Adversarial active learning for deep networks-A margin based approach；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）；
    6. Pytorch教程；
    7. 学术英语（网课）；
    8. 机器学习（网课）。
    
###### 2020/9/14
- 今日工作：
    1. 论文：Batch Active Learning With Two-Stage Sampling看完了;

###### 2020/9/15
- 今日工作：
    1. 跑代码：
    CIFAR10+ResNet-18+N-5_Rescent_RescentMax重跑3次

    [问题]
    每次重复跑的时候，没有删除model文件夹内容，使得准确率应该有提高，但这样跑应该不合理？是不是也有点合理。
    
    2. 画图：Average Accuracy-Number of Labeled Examples.+重复实验5次。

- 明日安排：
    1. 阅读完UML第四章（智能信息检索课）；
    2. 矩阵论作业；
    3. 实验总结报告；
    
###### 2020/9/16
- 今日工作：
    1. 论文:Adverarial Sampling for Active Learning看了1/3;
    2. 统计学习方法（李航）：logistic regression(二项/多项逻辑回归模型)；
    3. 书：understanding machine learning :from theory to algorithm第四章(uniform convergence)；
    4. 实验总结报告；
    
- 明日安排：
    1. 智能信息检索作业：
    (1). Chap 2 - p 41. 练习1，练习2
    (2). Chap 3 - p 50. 练习1， 练习3， 练习5，练习6，练习7，练习8.
    2. 论文：Adverarial Sampling for Active Learning；
    3. 矩阵论作业；
    4. 矩阵论（网课）；
    5. 统计学习方法（李航）；
    6. Pytorch教程；
    7. 学术英语（网课）；
    8. 机器学习（网课）。
    
###### 2020/9/17
- 今日工作：
    1. 学术英语（网课）；
    2. 论文:看到实验部分；
    3. 矩阵论作业：一题；
    4. 机器学习（网课）：课时71，72，随机初始化+NN训练步骤；
    5. 统计学习方法（李航）:最大熵模型前两节；
- 明日安排：
    1. 输出loss，增加loss prediction module，挑选样本。
    2. 论文；
    3. 智能信息检索作业：
    第2周作业：
    a. Chap 2 - p 41. 练习1，练习2
    b. Chap 3 - p 50. 练习1， 练习3， 练习5，练习6，练习7，练习8.
    第3周作业
    c. Chap4 - p.35 练习1，练习2.
    下周一之前阅读完第5章，周四前阅读完第6章
    4. 矩阵论作业；
###### 2020/9/18
- 今日工作：
    1. 论文：看完；
    2. 矩阵论作业OK；
- 明日安排：
    1. 输出loss;
    2. 论文:Learning to Sample: an Active Learning Framework；
    3. 智能信息检索作业：
    a. Chap 2 - p 41. 练习1，练习2
###### 2020/9/19
- 今日工作：
    1. 论文（LTS）:摘要+引言；
    2. 输出loss;
###### 2020/9/21
- 今日工作：
    1. 论文（LTS）：第二部分看完；
- 明日安排：
    1. 论文；
    2. 智能信息检索作业：
    a. Chap 2 - p 41. 练习1，练习2
    b. Chap 3 - p 50. 练习1， 练习3， 练习5，练习6，练习7，练习8.
###### 2020/9/22
- 今日工作：
    1. 论文(LTS):看完了;
    2. 智能信息检索：
    a. Chap 2 - p 41. 练习2;
    b. Chap 3 - p 50. 练习1;
- 明日安排：
    1. 论文；
    2. 智能信息检索作业：
    a. Chap 2 - p 41. 练习1，练习2
    b. Chap 3 - p 50. 练习1， 练习3， 练习5，练习6，练习7，练习8.
###### 2020/9/23
- 今日工作：
    1. 回顾论文LTS：boosting model看了一点；
    2. 矩阵论作业；
    3. 智能信息检索作业：
    a. Chap 3-p 50. 练习5，练习6；
- 明日安排：
    1. 回顾论文；
    2. 智能信息检索作业：
    a. Chap4 - p.35 练习1，练习2.
    b. Chap5 - p.41 练习1，练习2, 练习3
###### 2020/9/24
- 今日工作：
    1. 智能信息检索作业
    Chap3 - p 51. 练习3
    2. boosting model又看了一点；
- 明日安排：
    1. 组会记录；
    2. boosting model；
###### 2020/9/26
- 今日工作：
    1. 组会记录；
    2. boosting model；
    3. 论文；
    4. 智能信息检索作业
    Chap4 - p 59. 练习2
- 明日安排：
    1. 论文；
    2. 智能信息检索作业+论文；
    