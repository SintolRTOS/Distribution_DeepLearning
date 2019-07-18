本代码是“基于Tensorflow高阶API构建大规模分布式深度学习模型系列”文章的第三遍中介绍的内容的完整代码，文章以文本分类任务为例，详细介绍了如何创建一个基于Estimator接口的tensorflow模型，并使用`tf.estimator.train_and_evaluate`来完成模型训练和评估的完整过程。

## 使用说明

训练和测试数据打包在`dbpedia_csv.tar.gz`中，下载完整的代码目录，并解压`dbpedia_csv.tar.gz`，接着运行数据预处理任务：

```
python build_vocab.py
```

接着就可以训练和评估模型了：

```
python word_cnn.py --train_steps=20000
```


## 推荐阅读

1. [基于Tensorflow高阶API构建大规模分布式深度学习模型系列: 开篇](https://zhuanlan.zhihu.com/p/38470806)
2. [基于Tensorflow高阶API构建大规模分布式深度学习模型系列：基于Dataset API处理Input pipeline](https://zhuanlan.zhihu.com/p/38421397)
3. [基于Tensorflow高阶API构建大规模分布式深度学习模型系列: 自定义Estimator（以文本分类CNN模型为例）](https://zhuanlan.zhihu.com/p/41473323)

