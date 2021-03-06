<!---
markmeta_author: wongoo
markmeta_date: 2014-07-20 02:37:04
excerpt: 反思程序员找问题的思路
slug: classnotfound-problem
markmeta_title: 记一次ClassNotFound的问题
wordpress_id: 627
markmeta_categories: Experience
markmeta_tags: 思路,问题
-->

同事说，在台北部署一个项目时遇到一个ClassNotFound的问题，而开发环境就不会发生，问我可能的原因，我想可能是环境classpath没有包含jar或者有class重复之类的问题。 他检查了一下，除了开发环境是简体系统，部署环境是繁体系统之外，所有配置设定都一样。当时想java的项目，跟简体繁体应该没关系吧，应该还是其他地方的问题，但因为自己有事情忙没有帮他看这个问题。

第二天他告诉我找到原因了：ClassNotFound的问题是那个类初始化的时候会加载国际化内容，而项目中有配置简体国际化，但繁体的国际化没配置，导致读取国际化失败，类加载失败。添加了繁体国际化就解决了！

不管程序设计上是否有问题，单从找问题的思路上，我也犯了错误。因为一般情况遇到ClassNotFound的问题都是classpath的问题，在此遇到这样的问题，习惯性的认为就是这样的原因造成。没有更进一步思考发生错误可能的原因还有其他情况，比如类加载失败等； 另外是当得知只存在简体繁体OS之差的情况，没有从这个关键点去思考，没有去想程序逻辑是否跟系统的语言版本有关系。 看来以后遇到问题的时候，还要对问题进行深入的了解，了解问题本质以及尽可能多的原因。另外程序运行会存在依赖关系，在问题模拟时，存在任何差异都应该要引起注意，多思考一下这样的差异是否和程序逻辑有关系。

说到找问题，程序员往往都会犯一个错误：对自己写的程序盲目自信！觉得自己写的代码绝无BUG，出了问题，简单检查一下程序说没问题，就开始怀疑是不是framework有问题？更有甚者会怀疑JDK有bug，OS有bug。 当然也不是framework、JDK、OS就不可能有问题，要明白framework、JDK、OS都是经过长时间的验证，且大家都在使用，其他人都没有遇到问题，让你发现问题的几率还是很小的。项目实践证明，绝大多数问题都是程序逻辑的问题，framework的问题很难遇到，JDK、OS的问题几乎是没有！
