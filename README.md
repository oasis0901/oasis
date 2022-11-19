# oasis
一、数据预处理
（1）韵文
https://github.com/Werneror/Poetry 非常全的古诗词数据，收录了从先秦到现代的共计85万余首古诗词，从各朝代语料中等比例抽取训练集约10 万条，验证集5000 条，测试集5000 条。
（2）散文
		https://sites.google.com/site/xdguoxue/Home/guo-xue-jing-dian-quan-wen/jingshiziji%E2%80%94%E2%80%94sibuquanwen 经史子集——四部全文。爬虫获取语料约10 万条，抽取训练集约9 万条，验证集5000 条，测试集5000 条。
二、预训练模型
	本次实验预训练模型：
bert_Chinese: https://s3.amazonaws.com/models.huggingface.co/bert/bert-base-chinese.tar.gz
ERNIE_Chinese: http://image.nghuyong.top/ERNIE.zip
三、实验代码
	基于https://github.com/649453932/Bert-Chinese-Text-Classification-Pytorch项目的实验代码，更换数据集。（参考了钟雨玮同学中实验报告的注意事项）
四、实验结果
模型	acc	备注
bert	99.93%	单纯的bert
ERNIE	99.90%	ERNIE 是词汇级别的，在常见的中文处理任务上效果更优。
bert_CNN	99.89%	bert 作为Embedding 层，接入三种卷积核的CNN。

