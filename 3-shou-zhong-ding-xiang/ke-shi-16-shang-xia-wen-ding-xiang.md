它与行为定向相似，也是对用户打标签，但它所打的是一个即时标签，但实现它的系统，是不可能做到实时的，我称它为一个Near-line的系统，意思是接近实时的系统。

要对上下文打标签，需要一个Key是URL，Value是特征的Cache。广告投放系统就通过URL从这个Cache中取得相应的特征。实现这个Cache与搜索中的爬虫有些区别，因为无法预先知道哪些页面会出广告，如果用爬虫就会做很多无用功。所以在初始化的时候，Cache是空的。

Near-Line系统，这里不多介绍。

![](/assets/16.jpg)
