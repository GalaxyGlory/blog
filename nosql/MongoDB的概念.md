### MongoDB的概念

* Mongodb
* mongo
* 索引
* 集合
* 复制集
* 分片
* 数据均衡

### MongoDB的搭建

* 搭建简单的单机服务
* 搭建具有冗余容错功能的复制集
* 搭建大规模数据集群
* 完成集群的自动部署

### MongoDB的使用

* 最基本的文档的读写更新删除
* 各种不同类型索引的创建与使用
* 复杂的聚合查询
* 对数据集合进行分片，在不同分片间维持数据均衡
* 数据备份与恢复
* 数据迁移

### MongoDB运维

- 部署MongoDB集群
- 处理多种常见的故障
  - 单节点失效，如何恢复工作
  - 数据库意外被杀死如何进行数据恢复
  - 数据库拒绝服务时如何排查原因
  - 数据库磁盘快满时如何处理

![1533194386109](https://github.com/galaxyglory/blog/tree/master/nosql/MongoDB/Pictures/1533194386109.png)

![1533194494382](https://github.com/galaxyglory/blog/tree/master/nosql/MongoDB/Pictures/1533194494382.png)

![1533194534504](https://github.com/galaxyglory/blog/tree/master/nosql/MongoDB/Pictures/1533194534504.png)

![1533194555229](https://github.com/galaxyglory/blog/tree/master/nosql/MongoDB/Pictures/1533194555229.png)

![1533194572682](https://github.com/galaxyglory/blog/tree/master/nosql/MongoDB/Pictures/1533194572682.png)

```
mongo 127.0.0.1:27017/test
use admin
db.shutdownServer()
```
