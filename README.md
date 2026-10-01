# 鸿蒙开发编码和安全规范 (HarmonyOS-Dev-Standards)

> 持续收集并积累 HarmonyOS（鸿蒙）开发过程中的编码规范与安全规范，
> 构建可检索、可追溯、可演进的规范知识库。

## 项目目的 / Purpose

本项目是一个**知识库工程**：把 HarmonyOS 应用/系统开发中沉淀的
**编码规范（Coding Standards）** 与 **安全规范（Security Standards）**
持续收集、结构化归档，并通过 ArchiMate 意图图（ARGO）对外提供语义检索。

- **收集**：从官方文档、内部评审、代码审计、漏洞案例中提炼规范条目。
- **积累**：规范以意图图元素为权威载体，支持增量演进与版本追溯。
- **复用**：作为联邦成员对外开放规范能力，供其他项目按引用读取。

## 知识库结构 / Knowledge Base

| 位置 | 说明 |
| --- | --- |
| `design/KG/SystemArchitecture.json` | 权威意图图（默认 ArchiMate 3.2 本体），规范条目的唯一真源 |
| `docs/` | 面向人类的索引与说明（正文以意图图为准） |
| `docs/coding/` | 编码规范分类索引 |
| `docs/security/` | 安全规范分类索引 |

> 依据 ARGO「KG-first 存储」原则：规范**正文**存放在意图图元素中，
> `docs/` 仅保存面向上层阅读的索引、导航与摘要。

## 本体 / Ontology

采用 ARGO **默认本体（ArchiMate 3.2 + ARGO 扩展）**，不使用自定义 schema 包。

## 接入 / Onboarding

本项目是「阿米（Army）」组织的成员工程，并注册于联邦中心：

- 组织成员身份：`Business Actor` — HarmonyOS-Dev-Standards
- 联邦身份：`.argo/federation.json`（`projectId / sourceRepo / centerUrl / branch`）

## 贡献 / Contributing

1. 规范条目先进意图图（`addElement`），并归属到合适的 View。
2. 每条规范配一条可执行的 GIVEN-WHEN-THEN 验收说明。
3. 提交后登记 commit id 与相关文件路径。
4. 保持内容无重复：先查重（reuse），再新增。
