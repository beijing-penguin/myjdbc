源码贡献者<br />
北京-null，北京-企鹅<br />

##轻量级orm持久层操作api，只依赖commons-logging日志架包<br />
##支持ORACLE，MYSQL，SQL Server等数据库<br />
##采用低耦合分层软件架构：每层中，如operate，sqlhandle等包中的任何一个类都可以单独拿出来使用，基本无任何依赖<br />
##支持多数据源操作
##支持无缝对接当当开源的分库分表sharding-jdbc
##保证多数据源情况下的基本的跨库事务的有效性，如果是像mysql这种支持跨库事务的数据库，那么跨库事务会完全有效；如果是数据库的分布式存储（库不在同一个实例里面），那么本框架只保证基本的事务操作，但无法保证数据的最终一致性，这方面请自行考虑最大努力送达和TCC事务机制，大多数情况下能根据业务情况很好的处理数据不一致问题。

#注意事项
##本框架对jdbc操作轻量级封装，主要用于调试方便，开发方便，保证源码的可维护性。考虑到缓存命中率的问题，性能优化方面可以请根据自身业务需求的特点考虑自定义一级或二级缓存也许会更好。另外使用本框架源代码出现任何问题造成的经济损失，本人以及源码贡献者将不承担任何法律责任。

#联系方式
##QQ：429544557
##邮箱：429544557@qq.com
