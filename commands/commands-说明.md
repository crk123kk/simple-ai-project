## commands 是什么

## 可以有哪些 commands

/plan

让 AI 先做架构设计：

/planning
分析需求
输出：

- 技术方案
- 风险点
- 数据结构
- 页面结构
- API设计
  /implement

只负责实现：

/implement
严格按照 plan 实现
不要修改架构
/review

代码审查：

/review
检查：

- 性能
- 安全
- 类型
- 重复逻辑
- 边界条件
  /refactor

重构：

/refactor
目标：

- 降低耦合
- 提高复用
- 减少重复
  /debug

自动排查：

/debug
分析：

- 报错原因
- 调用链
- 修复方案
- 是否存在副作用

/prd

生成 PRD：

/prd
生成：

- 用户场景
- 功能列表
- 页面流程
- MVP范围
  /task

自动拆任务：

/task
将 PRD 拆成：

- 前端任务
- 后端任务
- AI任务
- 测试任务
  /architecture

生成系统设计：

/architecture
输出：

- 架构图
- 服务划分
- 数据流
- 缓存策略
- 部署方案

4. AI Coding 最强的一类：Project Knowledge

这类不是 command。
但价值远高于 command。

比如：

/project
/docs
/context
/knowledge

核心思想：

让 AI：

理解整个项目
理解业务
理解数据库
理解规范
理解历史代码

否则 AI 永远只是“单文件生成器”。

/ship

自动：

改代码
跑测试
修复 lint
提交 git
写 changelog
/research

自动调研：

/research AI photo restoration

输出：

竞品
技术方案
开源项目
API
商业模式
/generate-saas

现在很多 AI Agent 已经开始：

/generate-saas

自动生成：

landing page
auth
payment
dashboard
database
SEO
blog

-- 很多 command 本质就是 Prompt 模板。

例如：

/explain-like-senior
/explain-simple
/write-clean-code
/output-mermaid
/output-json

其实是：

Prompt 工程标准化

7. 真正顶级玩家在做什么

不是“收集 command”。

而是：

建立自己的 AI Engineering System

例如：

需求
↓
/prd
↓
/task
↓
/architecture
↓
/plan
↓
/implement
↓
/review
↓
/test
↓
/ship

这已经是：

AI 软件工厂。

8. 现在社区里比较出名的 command 方向

你可以重点研究：

方向 核心
Cursor Rules 项目规范
Claude Code Commands 工作流
OpenCode Skills Agent能力
OpenClaw Skills 自动化能力
RooCode Modes 多角色AI
Cline Tasks 自动执行
Devin Flow AI工程师
Aider Architect Mode 架构模式

## 修复编译器 报错 lint
