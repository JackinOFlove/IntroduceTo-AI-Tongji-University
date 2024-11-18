<h1>同济大学软件学院2024年春人工智能导论课程</h1>
## 1. 研究报告

+ 结合课堂内容并查阅人工智能领域相关研究方向（监督学习、无监督学习、强化学习等）的发展背景与技术现状，撰写总结文档。内容可包括：1）摘要，300字以内；2）人工智能总体发展历史，500字以内；3）相关研究方向技术发展趋势，500字以内，画一个发展趋势图；4）相关研究方向应用场景，500字以内；5）总结，300字以内；6）参考文献等）

## 2. 神经网络计算

+ 现有一个卷积神经网络，网络各层设置如下表第一列所示。

  请写出每层对应的输出数据维度以及各层参数量。

  数据维度请按H×W×C格式填写，其中 H,W,C 分别为数据的高、宽、通道数。

  如无特别说明，CONV和FC层均有bias。

  符号说明：

  - CONV k-N 表示卷积核大小为k×k，卷积核个数为N的卷积层，padding为1，stride为1；
  - POOL-n 表示n×n的max-pooling层，stride为n，padding为0；
  - FC-N 表示全连接层，输出维度为N。

  | 网络层     | 数据维度 | 参数量包括weights和biases |
  | ---------- | -------- | ------------------------- |
  | 输入       | 28×28×3  | 0                         |
  | CONV 3-16  |          |                           |
  | Leaky ReLU |          |                           |
  | POOL-2     |          |                           |
  | CONV 3-32  |          |                           |
  | Leaky ReLU |          |                           |
  | POOL-2     |          |                           |
  | FLATTEN    |          |                           |
  | FC-10      |          |                           |

## 3. 强化学习DQN

+ 利用网络资料，进行DQN（Deep Q-Learning）代码实现（也可实现其他强化学习模型），撰写实验报告PPT，并录制PPT的讲述视频（提交实验报告PPT+PPT讲述视频+readme文件+code，压缩后按照作业文档命名格式提交canvas；实验报告PPT包括算法流程介绍、实验结果分析，readme文件说明如何运行你的程序）。
+ 参考文献

​	Playing Atari with Deep Reinforcement Learning，https://arxiv.org/abs/1312.5602

​	github.com/floringogianu/atari-agents

## 4. 大语言模型部署

参考视频教程（附件1&2），在魔搭平台上部署并测试大语言模型，并完成报告。具体包括：

1. 登录并使用魔搭平台，注册时需要关联阿里云账号来获得免费的CPU云计算资源；
2. 通过Jupyter Notebook或者相应环境镜像进入相应的项目部署环境，根据相应模型的部署文档完成模型的部署；
3. 针对2-3个不同的模型（参考补充材料1）进行一些应用场景（比如问答，可参考补充材料2，也可自行设计问题）的测试，并开展不同模型之间的横向对比；
4. 报告需要包含：1）完成git clone相关git的截图或部署完成的相关截图 2）问答测试结果的相关截图 3）大语言模型之间的横向对比分析；
