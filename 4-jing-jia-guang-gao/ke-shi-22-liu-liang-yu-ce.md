在前面合约式广告中提到过合约式广告中有三个基本技术，1. 受众定向，2. 点击预测，3. 流量预测。在这三个技术基础上才可以做Online Allocation，本节主要介绍流量预测。

在定向条件分的比较粗的情况下，流量预测是比较简单的，比如只对人群分了几十个类，那么只需要进行简单的统计就可以进行流量预测了。

这里只介绍一种简单的，但很有启发意义的方法。这种方法是将查询视为a，文档集是\(u,c\)的一个反向检索的过程。与之相对的是在广告检索的过程中，查询是\(u,c\)，文档集是a。这种方法对u或c进行检索，所检索出的数量也就是流量的大小。之所以要这样做的原因是，广告的定向条件的可能组合非常多，不可能通过简单的统计来完成。

因为\(u,c\)的联合空间规模过大，无法直接对联合空间进行处理，也没有必要这样。所以需要对u和c分别处理。即分别对受众和页面建索引，用广告进行索引，可以得到满足定向的受众和页面量分别是多少。



