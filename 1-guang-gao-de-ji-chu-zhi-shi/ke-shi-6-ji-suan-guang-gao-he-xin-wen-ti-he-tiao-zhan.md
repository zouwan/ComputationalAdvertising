广告主为a，媒体为c，受众体为u，广告计算的核心问题就是计算出a,u,c相关的ROI最高值。（课堂主要是要描述思想，对于公式表达细节就不太计较了）

![](/assets/3.jpg)

从**优化**角度看它：

* 特征提取：受众定向，即把u和c打上标签的过程。
* 微观优化：对一次展示进行优化，得到最好的广告，最关键的技术是CTR预测。
* 宏观优化：因为在线广告是用户，媒体，广告商三方博弈，所以竞价市场机制的设计非常重要。
* 受限优化：在量一定的情况下，怎么来优化质，在线分配就是这个问题。
* 强化学习：如何知道在新的广告主或新的用户群预测它的点击率，很直觉的想法是尝试，分配一定的流量给广告，看是男性用户点击率高还是女性。但是在尝试的过程中会损失一部分收入，因为不是按最优策略出广告的了。尝试的过程即探索，使用探索的结果即利用。
* 个性化重定向。

从**系统**角度涉及：

* 候选查询：要使用实时索引技术，使广告能很快地进入索引，很快指两个方面，新的广告要能尽快上线，广告预算用完的广告要尽快下线。
* 特征存储：在线高并发要用到一些No-Sql技术。
* 离线学习：很多时候要用到Hadoop。
* 在线学习：一些比较快的反馈，比如得到用户上一个搜索词，要用到流计算技术。
* 交易市场：要用到实时竞价。

在线广告计算的主要挑战有：

* 大规模（Scale）：线投放系统中的高并发挑战，响应速度在常见的web应用中可能是最高的。
* 动态性（Dynamics）：需要所建立的模型支持快速变化，比如涉及到CTR预测，那么模型参数是否能快变，特征是否能快速改变都是有挑战的。
* 丰富的查询信息\(Rich query\)
* 探索与发现\(Explore & exploit\)：用户反馈数据局限于在以往投放中出现过的\(a, u, c\)组合，需要主动探索未观察到的领域，以提高模型正确性。


