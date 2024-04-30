---
title: "Measuring Switching Costs and the Determinants of Customer Retention in Internet-Enabled Businesses: A Study of the Online Brokerage Industry"
excerpt: "What is IS? Theorizing the IT Artifact"
categories:
  - Empirical
tags:
  - Switching Cost
  - Electronic Market
journal:
  - ISR
---

>文章链接：[https://pubsonline.informs.org/doi/10.1287/isre.13.3.255.78][1]  
>作者：Pei-Yu Chen, Lorin M.Hitt  
>时间：Sptember 2002  
>期刊：ISR  
>总结：本文测量了切换成本，并探讨了切换成本的驱动因素。  
>个人观点：效用的奇妙用法。

## 摘要

The ability to retain and lock in customers in the face of competition is a major concern for online businesses, especially those that invest heavily in advertising and customer acquisition. In this paper, we develop and implement an approach for measuring the magnitudes of switching costs and brand loyalty for online service providers based on the random utility modeling framework. We then examine how systems usage, service design, and other firm and individual-level factors affect switching and retention. Using data on the online brokerage industry, we find significant variation (as much as a factor of two) in measured switching costs. We find that customer demographic characteristics have little effect on switching, but that systems usage measures and systems quality are associated with reduced switching. We also find that firm characteristics such as product line breadth and quality reduce switching and may also reduce customer attrition. Overall, we conclude that online brokerage firms appear to have different abilities in retaining customers and have considerable control over their switching costs.

## Introduction

公司往往会将大量投资用于吸引新客户，因为它们相信这些早期客户的获取投资会生成忠诚客户的长期利润流。这一策略的关键是，客户会经历某种“转换成本”，以防止其换到另外一个提供商。  
本文用数据实证测量了转换成本，并探讨了系统设计、客户特征、公司特征如何影响转换成本以及人员流失。

## Literature Review

### *Switching Cost*

Klemperer将转换成本分为三类：

1. 交易成本。指和供应商开始新关系的成本，也包含结束现有关系的成本。
2. 学习成本。指使用新产品达到和旧产品相同舒适度的成本
3. 人工转换成本。公司故意造成的，如重复购买折扣等
4. 其他成本：如风险规避、决策偏差等

经济学研究转换成本可以影响各种关键的竞争现象。  
市场营销研究影响品牌忠诚度的因素。  
IS采用经济学视角，但几乎没有关于系统变量如何影响转换成本的文献。

### *Electronic Market*

电子市场往往被认为有较低的转换成本，因为只需要点击一下即可。但公司引入了新的“摩擦”，包括用户资料个性化、点击奖励等，以实现留存客户。

## 核心构念和方法论

### 核心构念和假设

![Data screen]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2002-09-01-Measuring-Switching-Costs-p1.png)

重点关注*switching cost*和*attrition* ，参见上图的假设

### 估计切换成本

$u_j^i = \gamma_j + x_j \beta - r_j \alpha + z^i \lambda_j - \sum_{k=1}^Ms_kW_k^i +\epsilon_j^i$
{: style="text-align: center;"}

使用随机效应模型，其中$u_j^i$代表第$i$个人选第$j$个公司的效用，$\gamma_j$代表公司固定效应，$x_j$是非价格因素，$r_j$是价格，$z^i$是消费者特征，$W_k^i$是切换成本。

### 估计流失和转换驱动因素

和上式类似，不过把y换成行为的logit

## 结论

![Data screen]({{ site.url }}{{ site.baseurl }}/assets/images/posts/2002-09-01-Measuring-Switching-Costs-p2.png)

[1]: https://pubsonline.informs.org/doi/10.1287/isre.13.3.255.78
