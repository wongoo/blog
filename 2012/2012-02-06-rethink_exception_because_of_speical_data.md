<!---
markmeta_author: wongoo
markmeta_date: 2012-02-06 11:13:38
slug: rethink_exception_because_of_speical_data
markmeta_title: 反思异常数据导致项目运行异常问题
wordpress_id: 185
markmeta_categories: Inspiration
markmeta_tags: 项目管理,异常处理
-->

项目情况：
客户定制项目，客户提供的各种的数据规格未知。

遇到的问题：
因为未知的数据格式问题，导致系统异常不能使用。

反思原因：
因为项目开发中只考虑到了提供的测试数据的规则状况，忽视了异常数据会产生的漏洞。为修补问题话费了更多的人力，给客户留下不好的印象。

后续遇到类似问题应如何解决：
项目系统应该是始终能正常运行的，容错性良好的；系统不应该出现异常，应有错误处理机制；在设计开发阶段就应该考虑各种异常状况，提供异常提醒和处理机制。 
能够在异常机制能够处理范围内能解决的事情，则尽量少和客户沟通制定太多数据规则，在项目质量和可控性上能给客户良好的印象。

