# ent-workspace

`ent-workspace` 是 ent-loom 系列项目工作区，包含两个独立 Git 仓库。根目录只负责导航，不作为统一 Maven Reactor。

## 子仓库

| 仓库 | 定位 | Java 基线 | 文档 |
|---|---|---|---|
| [ent-loom](./ent-loom/README.md) | 实体建模与业务扩展框架 | JDK 21+ | [文档中心](./ent-loom/docs/index.md) |
| [ent-runtime](./ent-runtime/README.md) | 轻量应用运行时基础设施 | Java 8 | [运行时边界](./ent-runtime/docs/architecture/运行时边界.md) |

两个仓库独立构建、提交和发布，详细架构、边界和路线以各自文档为准。

## 版本口径

- `ent-loom` 主线和完整 Reactor 以 JDK 21+ 为基线；Core/Boot 2 的 Java 8、Boot 3/4 的 Java 17 属于独立兼容路线。
- `ent-runtime` 当前以 Java 8 源码和目标版本验证基础运行时能力。

根 README 只说明工作区结构，不重复维护子仓库的技术细节。
