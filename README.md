# Patent-Classification-Competition
This the code of the Patent Classification Competition, found by CCF &amp; Patsnap
## Update Log
这是2022年由CCF&Patsnap主办的专利分类大赛。  
我们在A榜实现了61.59%的正确率，在A榜截止前保持Top40 Nationwide。
我们主要探索了以下提分方法：

1. 测试不同的中文Bert模型，其中Mengzi的效果最佳；
2. 使用各种数据增强方法，包括互译、随机切分、随机删除和同义词替换；
3. 最终，我们选用了在专利文本上预训练的英文Bert模型，将中文语料翻译为英文后进行训练，在单个模型中效果最佳；
4. 使用集成学习的方法，将上述方法中训练出来的数个模型进行投票集成。

目前该项目的代码较为混乱，整理将会在数周后完成。