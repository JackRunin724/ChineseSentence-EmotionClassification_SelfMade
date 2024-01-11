# 中文语句情感分类（自制）ChineseSentence-EmotionClassification_SelfMade
## 需求
- transformers
- torch
- datasets
## 数据集
ChnnSentiCorp 数据集，已上传在项目中了。
## 模型
backbone 为 bert-base-chinese 预训练模型，下游任务模型为一个全连接网络。
## 训练
不对预训练模型进行训练，仅训练下游任务模型。
优化器使用 AdamW 优化器，Loss 函数使用交叉熵， 使用 HuggingFace 提供的线性学习率调节器。
