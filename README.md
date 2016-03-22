## 咔咔缓存（KakaCache）
> 咔咔一声，缓存搞定。这是一个专用于解决Android中网络请求及图片加载的缓存处理框架

## 项目目标
    本项目是作为实验项目，不保证其稳定性及可靠性
    因为缓存业务的复杂性，本项目尽可能适应更多的使用场景
    目前考虑到的，会实现的功能清单，会在下方依次罗列出来

### 缓存层级
- Internet临时缓存
- 磁盘缓存
- 内存缓存

### 缓存策略
- 仅缓存
- 仅网络
- 优先缓存
- 优先网络
- 先缓存后网络

### 缓存置换算法
- 先进先出算法（FIFO）：最先进入的内容作为替换对象
- 最近最少使用算法（LFU）：最近最少使用的内容作为替换对象
- 最久未使用算法（LRU）：最久没有访问的内容作为替换对象
- 非最近使用算法（NMRU）：在最近没有使用的内容中随机选择一个作为替换对象
- 其他算法，包括变种算法和组合算法

### 线程管理
- 支持多线程操作
- 支持UI线程回调

### 自动清理
- 缓存过期后，自动清理
- 容量不足时，清理冗余数据

### 配置项 - 约定大于配置
- 策略
- 容积
- 有效期
- 是否启用
- 置换算法
- 线程池大小
- 缓存实现

