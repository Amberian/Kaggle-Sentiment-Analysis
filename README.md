# Kaggle-Sentiment-Analysis
参考链接：https://github.com/BrambleXu/word2vec-movies 提交链接：https://www.kaggle.com/c/word2vec-nlp-tutorial
数据来源：https://www.kaggle.com/c/word2vec-nlp-tutorial/data

文件说明
---
1_bag of words (submit).ipynb： 先对数据进行预训练，包括去除HTML标签，去除数字和标点，去除停用词，词干提取和词形还原等，然后使用词袋模型，加上随机森林，但是效果不好
2_word2vec.ipynb：用gensim的word2vec训练词向量，并保存
2_word2vec_2.ipynb：导入上步的词向量，然后对使用Kmeans对词汇做聚类，使用类别的one-hot向量表示review，然后用随机森林对review进行训练和预测，准确率可以达到83.5%。也尝试了在获得词向量之后，取平均获得每个review的词向量，然后用随机森林，但是效果为83.0%。还是用上面那种比较好。
