# Transforming

**UC Berkeley的博士生Eric Tzeng发表在ICCV 2015上的文章《Simultaneous Deep Transfer Across Domains and Tasks》**

Motivation
作者提到了两种层次的transfer：

**domain transfer**：就是适配分布，特别地是指适配marginal distribution，但是没有考虑类别信息。如何做domain transfer：在传统深度网路的loss上，再加另一个confusion loss，作为classifier能否将两个domain进行分开的loss。两个loss一起计算，就是domain transfer。
**task transfer**：就是利用class之间的相似度，其实特指的是conditional distribution。类别之间有相似度，要利用上。类别之间的相似度：比如一个杯子与瓶子更相似，而与键盘不相似。文章的原话：it does not necessarily align the classes in the target with those in the source. Thus, we also explicity transfer the similarity structure amongst categories.

迁移学习其实是基于深度学习的原理，在进行训练的时候，前几层网络是会学习一些普遍存在的特征（如果是图像数据作为input，那）
