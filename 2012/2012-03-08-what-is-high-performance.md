<!---
markmeta_author: wongoo
markmeta_date: 2012-03-08 17:13:02
slug: what-is-high-performance
markmeta_title: 高性能系统思考－－何为高性能
wordpress_id: 228
markmeta_categories: Inspiration
markmeta_tags: high-performance,高性能
-->


高性能是相对低性能而提出的，低性能是指不能同时大量获取有限的资源，但高性能不是能够同时大量获得有限的资源，而是能够同时获得大量被‘认可’的资源。

那高性能系统的设计的目标就简单的变为：让有限的资源转变为大量‘认可’的资源。

这里要定义什么资源是值得认可的？如何产生大量认可资源？ 

‘认可’的意视具体系统而定，可以是指未过期、在可设定时间之类、在未改变之前、在未生效之前等等。。。

实现‘大量’的目的，方法可以是在数量上变多。前者方法思想总体来讲是一个multiple的思想，软件层面如多线程，多实例，多连接等，硬件方面如cluster。 

实现‘大量’的目的，方法也可以是让获取更容易。如添加缓存。
