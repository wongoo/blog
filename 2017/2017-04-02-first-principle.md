---
author: wongoo
date: 2017-04-02
title: 用第一性原理思考问题而不是类比
categories: experience
tags: thought,first-principle,methodology
---
---

#用第一性原理思考问题而不是类比

## 1. Musk关于第一性原理的故事

最近老罗在他的节目总讲到Elon Musk关于第一性原理的故事，从[网络](https://www.zhihu.com/question/21459243/answer/26326053) 上找到了这个故事的描述，摘取如下：

>在MUSK开发电动车案例中，有些人会说现在的电池组真的很贵，而且未来价格也不会低到哪去，因为它过去一直都是那么贵。这些人会说电池组每千瓦小时要烧掉600美元。而且未来也不会好到哪里去的。有史以来，成百上千的权威人士都声称一个行业、设计图样、一个实体或者一个想法都已经达到了它的顶峰。在这种思路的影响下，电池组再也没有改进的空间，或是以更低的成本生产出来。这些人说的话都被汹涌扑来的创新证明是无稽之谈。或者，他们可以拍屁股想出一些微不足道的改进。”

>然而从第一性原理出发，我们问：电池的材料构成都是什么?这些材料的现货市场价值是怎样的?电池是由碳、镍、铝、其他用于分离的聚合物还有一个金属罐组成的。如果我们去伦敦金属交易所购买这些金属材料，然后把这些材料分解一下，那么这些组成电池组的材料每种又值多少钱呢?

>Musk在采访中说道，他将电池组分解成最基础的材料组成部分：碳、镍、铝、其他用于分离的聚合物还有一个盒子。这些都是电池组重要的组成元素，这是形成一块电池的最基本的事实。从那里，每个部分都可以优化、改进，最终的优化程度也取决于解决问题这些人的聪明才智。于是，现在电池的价格就变成了每千瓦小时80美元。


## 2. 什么是第一性原理
Wikipedia有词条[First principle](https://en.wikipedia.org/wiki/First_principle)，第一句话就很清楚：
>A first principle is a basic, foundational proposition or assumption that cannot be deduced from any other proposition or assumption.

翻译：第一性原理是一个基础基本的命题或假设，它不能从其他的命题或假设推导出。

其主要应用于物理学中，表示从量子力学这个最基础的层面去计算物质的结构。

## 3. 第一性原理的意义
Elon Musk的例子是指要从电磁组成的基础材料去重新分析，了解电磁最根本的东西，才能了解电磁的关键成本，才能对电磁的生产进行优化，最终实现行业的变革。

一般人常常通过经验和类比的方式去看待一个事情。比如Elon Musk电磁的例子，常人只是拿过去电磁的成本很贵，电磁效率低下这些经验来评判电动车不可行。

经验和类比往往是一个很好的判断事情的方式，但在某些时候却可能一叶障目看不到事情本质。

比如，买股票这事情，很多股票推荐都是根据过往的经验，查看大盘状况，分析股票走势，根据一个变化规律的经验得出股票会涨，建议购买。这种方式买了可能会赚，也很有可能会赔。但巴菲特买股票，不回去分析股市走向，而是实实在在的去了解一个公司的经营状况、高管构成、市场前景等等一切影响股票的因素，从这些根本去分析计算公司会不会赚钱，如果能赚钱才会真正去买这只股票。

Elon Musk一直推崇的用第一性原理思考问题，而不是类比。用第一性原理去思考问题，才能真正解决问题。

## 4. 我对第一性原理的感受

从事软件编码过程中，常常遇到很多问题，我解决问题的一个方式常常是靠经验出发，看到一个问题信息，大概知道问题的原因。这在大多数情况下有用，能够直接解决问题。但计算机技术的问题常常看到的只是表象，而根本原因可能垮了很多层，饶了很多圈。靠经验去解决，往往会把人带到死胡同，百思不得其解。 这个时候需要转变思维方式，用第一性原理的方式去思考问题，了解问题后面的原理和流程，从根本原理和流程去分析问题，才可以找到问题的根本原因。

比如，有一次遇到一个系统没办法加载配置的问题，按照经验，第一想到什么改动影响了配置加载，但改动东西很多，就一个个还原试，但这样效率很慢；又打开debug调试分析，也看不到有价值的内容。最后重新思考配置加载的过程，加载配置所需要的依赖，从这个方向分析，发现是少了依赖包。而少了依赖包的原因不是本项目的修改导致，而是父项目重构更改了依赖方式导致。

经验往往是有用的东西，当经验快速走不通时，就得回头用第一性原理去思考了。



