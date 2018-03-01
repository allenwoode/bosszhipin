
-----------从Gitee（码云）迁移过来-----------

该项目主要包括BOSS直聘网站职位信息的爬取、入库以及可视化需求分析。相关内容已整理在知乎专栏（数据分析入门）：
https://zhuanlan.zhihu.com/p/32953098
https://zhuanlan.zhihu.com/p/33476271

网址采用城市+行业组合的方式，通过Scrapy框架进行爬取，并通过Peewee存储到数据库，数据量预期在两三百万左右，但是爬取一段时间后，BOSS直聘网站更新改版，最终数据量只有25万左右。

部分爬取数据显示如下：
![爬取信息1](https://github.com/lxm909055383/bosszhipin/blob/master/img/1.jpg)
![爬取信息2](https://github.com/lxm909055383/bosszhipin/blob/master/img/2.jpg)


基于这25万数据，目前已进行三个需求分析（主要基于数据分析、机器学习、人工智能相关行业）：
一、各城市对职位的需求量（包括总的公司数与提供的职位数）
![可视化](https://github.com/lxm909055383/bosszhipin/blob/master/img/3.jpg)

从上图可以分析出以下几点：
1.一线城市北上广深对人才的需求量还是远远高于其他城市，一个是政治中心、一个是经济中心、一个是珠三角省会、一个是经济特区，多年来的高速发展已经成滚雪球般的态势，发展越好，对于人才的需求也更大。
2.帝都北京稳居第一，远超其他三个一线城市，首先跟北京的特殊地位——首都有一定关系，其次互联网+、人工智能时代的到来使得互联网行业成为最热门的选择，而最早的一批互联网公司基本都在北京创立，这一行业的发展吸引了相应行业的人聚集，人的聚集又相应带动公司的聚集，两者相互影响使得北京成了互联网的主力军。
3.杭州一跃成为仅次于一线城市的人才聚集地，跟中国的转型（依靠科技创新）有着密切的关系，阿里巴巴、网易等知名互联网公司极大的提高了杭州的科技创新能力和第三产业的发展速度，加大了杭州对于人才的需求。
4.武汉、成都、西安等二线城市近年也有崛起之势，跟国家发展中西部的战略有很大关系，沿海一线城市逐渐趋于饱和，因为资源、面积、环境等各方面压力，国家有意向发展二、三线城市，武汉、成都、西安等城市凭借优良的地理位置，有非常大的发展空间，成为国家发展的首选，各种人才引进计划使得需求量逐日上升。

二、同职位（数据分析、机器学习、人工智能相关行业）在不同城市的薪资对比
![可视化](https://github.com/lxm909055383/bosszhipin/blob/master/img/4.jpg)

从上图可以分析出以下几点：
1.最直观的就是北京20K以上的职位数远远大于其他城市，接近第二位（杭州）的2倍，这也有力的支持了北京平均薪酬水平全国最高的观点，有报道北京地区平均薪资排名前十的行业中，互联网相关的行业就占据了较多的席位，如互联网/电子商务、IT服务(系统/数据/维护)等。
2.北上广深杭五个城市的低薪职位数量（5K以下）占比非常小，相比之下高薪（20K以上）职位数占有非常大的比例，高薪的诱惑也是近年来驱动相关从业者大量涌入这些城市的原因。
3.除北上广深杭这几个城市外，其他城市各档薪资职位数的分布较为均匀。
4.数据分析、机器学习、人工智能相关行业的职位绝大多数都集中在北上广深杭这些城市，其他城市提供相关行业的机会较少，可供选择的不多。

三、数据分析、机器学习、人工智能相关行业的关键词云图
![可视化](https://github.com/lxm909055383/bosszhipin/blob/master/img/5.jpg)

上面的词云图是根据数据分析、机器学习、人工智能相关行业的关键词生成的，字体越大，说明在所有关键词中出现的次数越多。从上图中，我们挑选出现次数最多的10个词语，分别为‘数据分析’、‘数据挖掘’、‘数据处理’、‘机器学习’、‘数据仓库’、‘MySQL’、‘python’、‘数据库’、‘Hadoop’、‘Hive’等，这说明相关职位对于求职者的技能要求大都体现在这些方面，可以有选择的进行学习。在此推荐几本相关的书籍：《深入浅出数据分析》、周志华的《机器学习》，Peter的《机器学习实战》，《数据挖掘：概念与技术》等。
