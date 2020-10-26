## resume
####  个人信息
 - 卞煜球/男/1994
 - 期望职位：大数据开发工程师
 - 技术博客：[https://muchen.cf](https://muchen.cf)
 - Github：[https://github.com/earthNoah](https://github.com/earthNoah)
 - 工作年限：3年
 - 本科/淮海工学院（江苏海洋大学）
 - 通信工程

---
#### 联系方式
 - 手机：18550032630
 - Email：[xiaoqiushiwo@gmail.com](xiaoqiushiwo@gmail.com)
 
---
#### 工作经历
##### 孩子王儿童用品股份有限公司 （ 2019年12月 ~ 至今 ）
##### 途牛旅游网 （ 2017年6月 ~ 2019年12月 ）

---
#### 技能评价
##### 大数据相关
 - 熟悉Flink、Flink Sql、Storm实时计算框架架构
 - 熟悉Hadoop、Kafka、Zookeeper大数据组件
 - 熟悉GreenPlum、TBase、Cassandra、HBase、Kudu分库式数据库
 - 熟悉Datax、cannal（binlog）、flume等数据传输工具的二次开发

##### 编程相关
 - 熟悉Java开发，了解多线程，GC垃圾回收
 - 熟练运用SpringMVC、SpringBoot、mybatis进行开发
 - 了解Dubbo、thrift、Akka、netty等rpc组件进行通信
 - 了解Python、Shell、Vue等语言
 
##### 其他方面
 - 熟悉在Linux环境进行troubleshooting
 - 了解RMDB如 postgresql、Mysql、Oracle、sql server、TIDB等
 - 了解测试工具如JMeter、postman等
 - 熟悉git、svn版本控制工具

##### 语言能力
 - 能够流畅阅读英文开源项目的技术文档和源码

---
#### 项目经验
##### 用户推荐系统 (途牛)
 - 目的:基于用户浏览产品协同过滤，产品相似度和产品流行度的推荐 
 - 技术栈: Flink+Redis+Kafka+Hbase
 - 工作内容:
	1. 通过 ABTest 方案，分场景/用户选择不同的算法，根据点击转化
	率，通过客观评测和主观评测选择更优的算法;
	2. 根据用户点击类型， 初始化用户下特征的权重和特征下用户的
	权重;
	3. 对历史特征的权重根据天数进行衰减;
	4. 响应用户反馈，吸引用户提供正确的反馈，修正推荐数据;
	5. 推荐poi目的地+主题产品+机票酒店+瀑布流+游记。
 - 工作成果：通过个性化接口替换途牛app、pc、m站，日均处理流量约1000w


##### 实时计算平台 （孩子王）
 - 目的:建设基于 Flink 的实时计算管理平台
 - 技术栈: Flink+Yarn+Spring mvc+Linux+Prometheus 
 - 工作内容:
	1. 框架开发:封装 Flink 代码，将对 env/source/sink 的操作封装
	到 jar 包中，采用可视化的方式进行配置，在运行时，通过反射
	获取用户代码片段，提交到 yarn 上运行，降低 Flink 开发成本;
	2. 项目开发:HDFS 日志分析项目，人脸+订单实时数仓项目等;
	3. 监控:kafka offset 监控，Flink 背压监控，Prometheus 中 mertic
	孩子王
	监控，FLink 日志统一推送 kafka 监控;
	4. 告警:通过短信，微信，邮件告警消费延迟告警，错误日志告警。
	5. 流计算代码 review:在自定义 source/sink 中是否有自定义的
	checkpoint 实现，时间语义是否正常使用，动态参数是否可以 提炼作为可配置的参数，日志打印是否存在循环打印导致日志暴 涨，常规的代码规范(sonar+findbug+alibaba code)。
 - 工作成果： 对接多个事业部，上线300+Flink

##### 数据中台研发 （孩子王）
 - 目的：为更好的建设TBase数据仓库，实现元数据管理、数据服务、数据地图和指标建模系统
 - 技术栈：SpringBoot+Vue
 - 工作内容：
 	1. TBase元信息维护、版本控制、表权限管控
 	2. 提供HTTP接口级别的服务对接异构数据库（ES、Mysql、TBase、PG、GP等）
 	3. 根据离线和实时任务生成数据血缘图
 	4. 根据主题、维度、度量、修饰词、描述词创建指标，实现建模功能
 - 工作成果：数仓研发、接口开发、产品、数据分析等一站式解决方案，维护1300+表，上线1300+接口

##### 其他实时项目
 - Flink 苔客广告项目(flume=>kafka=>mysql=>实时数仓)
 - Flink 实时数据直播间(kafka => window函数 => 根据城市+品类计算销量和点击)
 - Flink 流量解析项目(kafka => murmursHash(vt) => kafka)
 - Flink 我的浏览历史项目(kafka => window => HBase)
 - Flink 孩子王线上线下订单实时项目(binlog => window => trigger => KUDU => Redis => TMG | storm迁移 )
 - FLink HDFS日志解析项目(editlog => kafka => KUDU)
 - Storm 第三方广告项目 (kafka => 匹配 => Cassandra => TMQ) 
 - FLink SQL 营销工具服务订单宽表 (mysql => flink-cdc => ETL => kafka / => TBase )
 - FLink SQL 流量点击宽表 (mysql => binlog => ETL => 关联dim公司维表 Flink JDBC => TBase )


##### 其他Java项目
 - MVC-java 统一接口平台 (提供途牛推荐 + 机票 + 酒店 + 搜索 + 群体画像接口, 日请求 1000w+) 
 - MVC 大数据管理平台 (web + 多agent rpc调用, 实现动态扩容hadoop节点 + 监控服务 + 告警)
 - MVC 同步系统 (web + 多agent rpc调用, 通过datax实现异构数据库同步,已上线2000+任务) 

---

#### 兴趣爱好
 - 喜欢看博客，记笔记
 - 经常自学互联网新兴知识体系
 - 喜欢去户外骑自行车，旅游

