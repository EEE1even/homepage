# Unsupervised Pretraining for Sequence to Sequence Learning

用无监督方法来提高seq2seq的准确率

怎么做的：编码器和解码用两个语言模型的预训练权重进行初始化，然后用标注数据fine-tuned

之前方法的缺点：在缺少有监督训练数据时容易过拟合