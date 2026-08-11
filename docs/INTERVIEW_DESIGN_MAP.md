# Interview Design Map — jeecgboot__JeecgBoot

> 由 repo_fuse 自动生成（面试题库 × 本仓库设计映射）。用于把本项目的设计决策与面试高频设计主题对齐。

## 项目技术画像

- 框架/技术栈：Vue、Spring、Docker、Redis、MCP、RabbitMQ、PostgreSQL、React
- 文件规模：1809 个源文件
- 与面试题库命中 24 个设计主题

## 设计主题 ↔ 仓库实现映射

| 面试设计主题 | 仓库中的实现/证据 | 对应题库位置 |
|---|---|---|
| ReAct 与 Agent 工作流范式 | <内容命中> | 见题库「ReAct 与 Agent 工作流范式」概念笔记 |
| MCP | jeecg-boot/jeecg-boot-module/jeecg-module-demo/src/main/java/org/jeecg/modules/demo/mcp/McpDemoController.java, jeecgboot-vue3/src/views/super/airag/aimcp/AiragMcp.api.ts, jeecgboot-vue3/src/views/super/airag/aimcp/AiragMcpList.vue | 见题库「MCP」概念笔记 |
| Workflow 与自主 Agent 权衡 | <内容命中> | 见题库「Workflow 与自主 Agent 权衡」概念笔记 |
| LangGraph 与图编排 | jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/config/AuthStateConfiguration.java, jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/cache/AuthStateRedisCache.java, jeecgboot-vue3/tests/server/nodemon.json | 见题库「LangGraph 与图编排」概念笔记 |
| RAG 与知识库 | jeecgboot-vue3/src/views/super/airag/aiprompts/AiragExtDataList.vue, jeecgboot-vue3/src/views/super/airag/aiprompts/AiragExtDataExperiment.vue, jeecgboot-vue3/src/views/super/airag/aiprompts/AiragPrompts.api.ts | 见题库「RAG 与知识库」概念笔记 |
| 技能体系 | <内容命中> | 见题库「技能体系」概念笔记 |
| Prompt Engineering | jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/model/SysUserSysDepPostModel.java, jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/entity/SysUserDepPost.java, jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/service/ISysUserDepPostService.java | 见题库「Prompt Engineering」概念笔记 |
| Agent 记忆机制 | jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/monitor/controller/ActuatorMemoryController.java, jeecgboot-vue3/src/utils/cache/memory.ts | 见题库「Agent 记忆机制」概念笔记 |
| 上下文管理与压缩 | jeecg-boot/jeecg-boot-base-core/src/main/java/org/jeecg/common/util/SpringContextUtils.java, jeecgboot-vue3/src/views/demo/feat/context-menu/index.vue, jeecgboot-vue3/src/hooks/core/useContext.ts | 见题库「上下文管理与压缩」概念笔记 |
| 算法与 LeetCode | jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/entity/SysFillRule.java, jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/service/ISysFillRuleService.java, jeecg-boot/jeecg-module-system/jeecg-system-biz/src/main/java/org/jeecg/modules/system/controller/SysFillRuleController.java | 见题库「算法与 LeetCode」概念笔记 |
| 存储选型与状态持久化 | jeecg-boot/db/jeecgboot-mysql-5.7.sql, jeecg-boot/db/tables_nacos.sql, jeecg-boot/db/tables_xxl_job.sql | 见题库「存储选型与状态持久化」概念笔记 |
| Badcase 闭环与数据飞轮 | jeecgboot-vue3/src/views/monitor/trace/trace.api.ts, jeecgboot-vue3/src/views/monitor/trace/index.vue, jeecgboot-vue3/src/views/monitor/trace/trace.data.ts | 见题库「Badcase 闭环与数据飞轮」概念笔记 |
| 评测体系与 Benchmark | <内容命中> | 见题库「评测体系与 Benchmark」概念笔记 |

## 建议的面试切入点

- 本仓库最能体现设计深度的模块（按命中概念与证据文件定位，建议对照《项目内作答》准备）
- 每个主题准备"框架给的 vs 我设计的"对照（如用 LangGraph 则强调图结构与状态设计的自有决策）

---
生成时间：由 repo_fuse 生成，随题库/仓库变化可重跑更新。
