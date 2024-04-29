---
title: "A nearly perfect market? Differentiation vs. price in consumer choice"
excerpt: "Electronic marketplace lowers the buyers' search cost"
toc: true
toc_sticky: true
categories:
  - Empirical
tags:
  - Search Cost
  - Electronic Market
journal:
  - Quantitative Marketing and Economics
---

> 文章链接：[https://www.proquest.com/docview/865002175?sourcetype=Scholarly%20Journals][1]  
> 作者：Erik Brynjolfsson, Astrid A. Dick, Michael D. Smith  
> 时间：Nov 2009  
> 期刊：Quantitative Marketing and Economics  
> 总结：这篇文章建模并估计了搜索成本。通过对消费者异质性进一步分析，分析了差异化和价格因素与消费者搜索强度的关系。  
> 个人观点：为思考线上线下市场区别提供了一个本质参考：搜索成本

## 摘要

Internet shopbots allow consumers to almost instantly compare prices and other characteristics from dozens of sellers via a single website. We estimate the magnitude of consumer search costs and beneﬁts using data from a major shopbot for books. For the median consumer, the estimated beneﬁt from simply scrolling down to search lower screens is $6.55. This amounts to about 60% of the observed price dispersion and suggests that consumers face signiﬁcant search costs, even in this “nearly-perfect” market. Price elasticities are relatively high compared to ofﬂine markets (−7 to −10 in our base model). Furthermore, contrary to the common assumption, search intensity is not correlated with greater price sensitivity. Instead, consumers who search multiple screens put relatively more weight on non-price factors like brand.

## 数据

![Data screen]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p1.png)

参见上图，数据来自DealTime.com，一个著名的在线比较购物服务网址。该网址可以根据消费者的搜索，返回多个零售商的报价，默认按总价（包括除了基础商品价格，还有物流等各种价格）排序。一个屏幕最多返回10个结果，因此如果消费者往下划，即为进行搜索，付出了搜索成本。

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p2.png)

数据字段见上图，是以每个搜索结果中的一条为数据单元的。  

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p3.png)

进一步根据消费者搜索行为，可以将其区分为以上四种类型。

1. First screen consumer：只点击默认屏幕的消费者
2. Low screen consumer：滚动到下面屏幕点击的消费者
3. Multiple click consumer：点击多个优化的消费者
4. Sorting consumers：按总价以外排序的消费者

## 本文关注点

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p4.png)

将消费者异质性划分为两个维度：异质性口味，搜索成本上限。可以看到，若消费者有较高的异质性需求，以及较低的搜索成本，它会倾向于多搜索。有较低异质性需求，较高的搜索成本时，倾向于减少搜索。  
当异质性需求很高时，消费者往往会更少关注价格因素，其搜索行为的价格敏感性较低。

## 实证模型

### 基本模型

$u_{ij} = z_j * \theta + \epsilon_{ij}${: style="text-align: center;"}  
$p_j = logit(u_{ij})${: style="text-align: center;"}  
其中$i$代表消费者，$j$代表报价，$z_j$代表产品特征，包括价格和其他属性。  

### 随机系数模型

$u_{ij} = z_j * \theta + \sum_{k}{\sigma_kz_{jk}v{ik}} + \epsilon_{ij}${: style="text-align: center;"}  
$p_j = logit(u_{ij})${: style="text-align: center;"}  
该模型允许系数$\theta$随着消费者不同而不同。  

### 搜索收益和搜索成本上限

令第一个屏幕给消费者的剩余是$S_{s-1}(p_t, x_t; \theta)$，整个报价集的剩余是$S_{s}(p_t, x_t; \theta)$，则二者之差为消费者得到的搜索收益  
考虑到当且仅当消费者的期望收益大于搜索成本时，消费者才会搜索。因此，上面的搜索收益也是消费者搜索成本上限。

## 实证结果

### 系数

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p5.png)

如上图，first screen价格系数最高，代表了更大的价格敏感性。其他类型消费者会关注配送时间、品牌等信息。

### 价格弹性

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p6.png)

通过对logit模型对价格求弹性，得到上表。请注意，由于随机模型中每个消费者都有自己的系数，因此可以对所有消费者统计其价格弹性分位数。

### 搜索收益

![Summary statistics]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2009-11-01-A-Nearly-Perfect-Market-p7.png)

[1]: https://www.proquest.com/docview/865002175?sourcetype=Scholarly%20Journals
