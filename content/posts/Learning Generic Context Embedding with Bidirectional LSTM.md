# Learning Generic Context Embedding with Bidirectional LSTM

通用上下文嵌入在双向LSTM中的应用

context representation  上下文表示

sentence completion  句子补全

**之前的上下文表示有什么问题？**

不包括任何优化整个句子上下文整体表述的机制

个人理解，之前的方法将句子转换成向量后，这个向量就是定死的不会再改变，不会随着上下文的理解变化向量的表示方式或是范围



**文章想做什么？**

想从标签单词（target word）和其相关的句法上下文(sentential context)中获得更多的信息，最好是减少词嵌入时两者之间的依赖性



**怎么做？**

使用双向LSTM

**目标：**需要为围绕目标词的变长句式语境训练一个通用的任务无关的嵌入函数

![](src\context2vec) )

其他的模型只考虑将target词嵌入作为主要输出，context2vec专注于上下文表示，分配相似的embedding给上下文句子和句子中的标签
