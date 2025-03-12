# 项目介绍
这里是一个基于 Spring Boot + Redis 的简易秒杀系统 Demo，重点实践 缓存优化 和 并发控制，以保证高并发环境下的稳定性和性能。

# 技术栈
- **Spring Boot**（构建 Web 服务）
- **Redis**（缓存库存、减少数据库压力）
- **Redisson** 分布式锁（防止超卖）
- **MySQL**（存储秒杀订单）
- **LUA 脚本**（减少 Redis 请求，提高性能）

# 功能需求
1. **商品秒杀**：限制库存，确保不会超卖。
2. **高并发优化**：使用 Redis 缓存库存、Lua 脚本减少 Redis 交互、Redisson 进行分布式锁控制。
3. **数据库优化**：订单异步落库，减少数据库压力。


