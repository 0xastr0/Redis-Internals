# Redis Internals![image title](http://www.zpoint.xyz:8080/count/tag.svg?url=github%2FRedis-Internals-CN)

* [English](https://github.com/zpoint/Redis-Internals/blob/5.0/README.md)
* 如果你需要接收更新通知, 点击右上角的 **Watch**, 当有文章更新时会在 issue 发布相关标题和链接

这个仓库是我分析 [redis](https://github.com/antirez/redis) 源码时做的记录

```c
# 基于版本 5.0.5
cd redis
git fetch origin 5.0:5.0
git reset --hard 388efbf8b661ce2e5db447e994bf3c3caf6403c6

```

# 目录

* [基本对象](#基本对象)
* [服务](#服务)
* [为什么创建这个仓库](#为什么创建这个仓库)
* [学习资料](#学习资料)
* [参与贡献](#参与贡献)
* [授权](#授权)

# 基本对象
 - [x] [字符串/string(sds)](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/sds/sds_cn.md)
 - [x] [哈希/hash(ziplist/ht)](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/hash/hash_cn.md)
 - [x] [列表/list(quicklist)](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/list/list_cn.md)
 - [x] [集合(intset/ht)](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/set/set_cn.md)
 - [x] [有序集合(ziplist/skiplist/ht)](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/zset/zset_cn.md)
 - [x] [hyperloglog](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/hyperloglog/hyperloglog_cn.md)
 - [x] [streams](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/streams/streams_cn.md)
 	- [x] [rax](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/rax/rax_cn.md)
 	- [x] [listpack](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/listpack/listpack_cn.md)
 - [x] [geohash](https://github.com/zpoint/Redis-Internals/blob/5.0/Object/geohash/geohash_cn.md)

# 服务
- [x] [持久化](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/persistence/persistence_cn.md)
- [x] [发布订阅(pubsub)](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/pubsub/pubsub_cn.md)
- [x] [cluster](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/cluster/cluster_cn.md)
	- [x] [reshard](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/cluster/cluster_cn.md#reshard)
	- [x] [gossip](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/cluster/gossip/gossip_cn.md)
	- [x] [failover](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/cluster/failover/failover_cn.md)
- [ ] [replica](https://github.com/zpoint/Redis-Internals/blob/5.0/Server/replica/replica.md)
- redlock
- protocol
- transaction

# 为什么创建这个仓库

* 出于学习目的
* 在 [学习资料](#学习资料) 中有非常棒的中文书籍可以参考, 但是没有类似的英文资料
* [Redis 设计与实现](http://redisbook.com/) 一书当前是基于 redis 3.0 版本的(我读的时候是旧版 基于2.x版本), 即使是 redis 3.0 到当前版本许多实现细节也发生了变化

# 参与贡献学习资料
* [Redis 设计与实现](http://redisbook.com/)
* [Redis Documentation](https://redis.io/documentation)
* [Redis 5.0 RELEASENOTES](https://raw.githubusercontent.com/antirez/redis/5.0/00-RELEASENOTES)

## 参与贡献

欢迎所有形式的贡献

* 提交一个 pull request
  * 如果你想分享任何你知道的相关知识
  *  发布一篇文章
  * 更正技术性错误
  * 更正语法性错误
  * 翻译
  * 其他情况, 不限于上述
* 提交一个 issue 
  * 任何建议
  * 任何问题
  * 更正错误
  * 其他情况, 不限于上述

# [授权](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)