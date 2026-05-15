# Skill List

本仓库包含的 Claude Code Skills 清单。

---

## 应用构建

| Skill | 说明 |
|-------|------|
| **artifacts-builder** | 构建 claude.ai HTML Artifacts，使用 React 18 + TypeScript + Vite + Tailwind CSS + shadcn/ui，开发后打包为单个自包含 HTML 文件 |
| **web-artifacts-builder** | 与 artifacts-builder 功能一致，构建多组件 HTML Artifacts 的另一版本 |

## 文档处理

| Skill | 说明 |
|-------|------|
| **document/docx** | 创建、读取、编辑 Word (.docx) 文档，支持表格、图片、页眉页脚、批注、目录等 |
| **document/pdf** | 全面的 PDF 处理：读取/提取文本与表格、合并/拆分/旋转页面、加水印、创建新 PDF、填表单、加解密、OCR |
| **document/pptx** | 创建和编辑 PowerPoint (.pptx) 演示文稿，支持模板编辑（解包 XML）、从头创建（pptxgenjs），含设计规范 |
| **document/xlsx** | 使用 pandas + openpyxl 创建/编辑/分析 Excel (.xlsx)，强制使用 Excel 公式而非硬编码，含财务建模规范 |
| **doc-coauthoring** | 三阶段协作写作流程：收集上下文 → 逐节精炼结构 → 读者测试（用新 Claude 实例盲审），产出高质量文档 |

## 开发工具

| Skill | 说明 |
|-------|------|
| **commit** | 智能 commit 工作流，自动生成 emoji + Conventional Commits 格式消息，检测 pre-commit hooks，从分支名提取任务 ID，建议拆分多逻辑变更 |
| **changelog-generator** | 从 git 历史自动生成用户友好的 Changelog，分类变更（功能/改进/修复等），将技术 commit 消息转化为清晰的发版说明 |
| **frontend-design** | 创建独特、生产级的前端界面，强调大胆的美学选择，避免"AI slop"式通用设计，注重排版、色彩、动效和空间构图 |
| **webapp-testing** | 使用 Playwright 交互式测试本地 Web 应用，支持验证前端功能、调试 UI、截图、查看浏览器日志 |
| **mcp-builder** | 创建高质量 MCP Server 的完整指南，四阶段流程：调研规划 → 实现（Python/Node）→ 审查优化 → 编写评估用例 |

## 外部集成

| Skill | 说明 |
|-------|------|
| **connect** | 通过 Composio Tool Router 连接 1000+ 外部应用（Gmail、Slack、GitHub、Notion 等），让 Claude 执行真实操作（发邮件、建 Issue、发消息） |
| **connect-apps** | connect 的插件版本，使用 `composio-toolrouter` 插件连接 1000+ 应用，提供引导式安装、设置和 OAuth 授权流程 |

## 效率与发现

| Skill | 说明 |
|-------|------|
| **find-skills** | 从开放技能生态 (skills.sh) 发现和安装 Skills，搜索、验证质量（安装量/来源信誉）后呈现可安装选项 |
| **skill-creator** | 元技能：创建和迭代改进新 Skill。包含意图捕获、SKILL.md 编写、子代理测试、评分、人类反馈 UI、迭代优化等完整流程 |

## 专项工具

| Skill | 说明 |
|-------|------|
| **tailored-resume-generator** | 分析职位描述，生成针对性简历，提取关键要求与关键词，映射候选人经验，优化 ATS 兼容性，提供差距分析和面试建议 |
| **twitter-algorithm-optimizer** | 基于 Twitter 开源算法（Real-graph、SimClusters、TwHIN、Tweepcred）分析优化推文，最大化正向互动信号 |
| **video-downloader** | 下载 YouTube 视频，支持多画质（1080p/720p/480p/360p）、多格式（mp4/webm/mkv）和纯音频 MP3，自动安装 yt-dlp |
