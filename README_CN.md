# RhythmAntiCheat
基于 lightanticheat 的分支项目。<br>
**支持的 MC 版本**：1.8 至 1.21，同时兼容 Folia、Geyser 及 [其他插件](F-A-Q.md)。

## 相关链接
* 更精确的配置方案：[MILKv2 的配置文件](https://github.com/MILKv2/lightanticheat-config)

## 贡献指南
请查阅 [CONTRIBUTING.md](CONTRIBUTING.md) 文件获取更多信息。

## 文档说明
### 核心特性：
* 精准检测机制，极低误报率
* 多线程优化代码，运行稳定高效
* 无需额外依赖库或插件
* 多数检测模块兼容 Geyser
* 支持 Folia 服务端
* 提供 Discord 通知的 Webhook 支持
* 为管理员提供便捷的实用工具

### 命令列表：
| 命令 | 功能描述 |
|------|----------|
| `/light reload` | 重载插件配置 |
| `/light teleport` | 传送至作弊标记位置 |
| `/light checks` | 显示所有已启用/禁用的检测模块 |
| `/light alerts` | 切换警报开关状态 |
| `/light tps` | 显示插件计算的 TPS |
| `/light client` | 显示玩家客户端品牌 |
| `/light ping` | 显示玩家延迟及连接稳定性 |
| `/light cps` | 显示玩家点击频率 (CPS) |

### 权限节点：
| 权限节点 | 功能说明 |
|----------|----------|
| `lightanticheat.checks` | 使用 `/light checks` 命令 |
| `lightanticheat.reload` | 使用 `/light reload` 命令 |
| `lightanticheat.alerts` | 继承所有警报相关权限 |
| `lightanticheat.alerts.notify` | 接收调试信息通知 |
| `lightanticheat.alerts.toggle` | 使用 `/light toggle` 命令 |
| `lightanticheat.alerts.teleport` | 使用 `/light teleport` 命令 |
| `lightanticheat.tps` | 使用 `/light tps` 命令 |
| `lightanticheat.ping` | 使用 `/light ping` 命令 |
| `lightanticheat.client` | 使用 `/light client` 命令 |
| `lightanticheat.cps` | 使用 `/light cps` 命令 |
| `lightanticheat.bypass` | 绕过所有检测机制<br>（可在配置中启用具体模块的绕过权限） |
| `lightanticheat.*` | 获取所有上述权限 |

## Maven/Gradle 集成
#### Maven 依赖：
```xml
<dependency>
  <groupId>me.vekster</groupId>
  <artifactId>lightanticheat</artifactId>
  <version>1.2.7</version>
</dependency>
