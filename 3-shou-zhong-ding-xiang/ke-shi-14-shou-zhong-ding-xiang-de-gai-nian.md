受众定向是指按人群来划分对广告的售卖和优化，它是在线广告中最核心的部分。受众定向是在线广告区别于线下广告最本质的部分。

受众定向是为ROI优化中打标签的过程，它是对Ad，User，Context打标签。受众定向中有一种特殊的定向，上下文标签，即通过用户所浏览的网页，判断用户的兴趣。这种定向一般认为是上下文定向，但个人认为上下文标签也可以认为是用户即时的兴趣或是标签。

标签有两大主要作用：1.建立面向广告主的流量售卖体系，这一点本身就决定了标签不能按系统优化的思路来设计，即所打的标签一定要能被广告主理解。比如对上下文打标签，要对页面进行分类，个人认为更有效的方式是对页面进行supervise learning，即预先定义好标签体系，然后对页面进行分类，而不应该直接用聚类的方法或是Topic Model的方法打出一些无法直接解释的标签，因为无法对广告主进行售卖。这点是广告与其它用户产品不同的地方。2.为各机器学习模块（如CTR预测）提供原始特征，比如提供性别，年龄等特征供机器学习分析。

举一个例子来说明什么是一个标签体系，广告有三个轴，User，Ad，Context。

![](/assets/13.jpg)

受众定向方式，我们基本可以分为三类。1.对user和feature，2.对context和feature，3.对Ad和User的组合打标签，即在特定的广告主条件下，用户应该打什么标签，这种标签就引出了我们后面要讲的Demand方的Audience Segmentation，即根据广告主的逻辑给用户打标签。

