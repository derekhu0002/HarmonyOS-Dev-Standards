# 规范知识库索引 / Standards Index

本目录保存**面向人类**的索引与导航。规范的**权威正文**存放于意图图
`design/KG/SystemArchitecture.json` 的元素描述中（ARGO KG-first 存储原则）。

## 分类 / Categories

| 目录 | 主题 | 权威来源 |
| --- | --- | --- |
| [`coding/`](./coding/README.md) | 鸿蒙编码规范（ArkTS / ArkUI / 工程结构 / 命名 / 性能） | 意图图元素 |
| [`security/`](./security/README.md) | 鸿蒙安全规范（权限 / 数据安全 / 加密 / 隐私 / 组件安全） | 意图图元素 |

## 使用方式 / How to use

- 检索：通过 ARGO 语义检索（`getSystemArchitecture` / `memory_search`）按意图查询规范。
- 阅读：以 `docs/` 的索引定位分类，再到意图图读取条目正文。
- 扩展：新规范先查重（reuse），再新增为意图图元素并登记 commit。
