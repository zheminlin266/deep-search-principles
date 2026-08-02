# 深度搜索原则（Deep Search Principles）

[![skills.sh](https://skills.sh/b/zheminlin266/deep-search-principles)](https://skills.sh/zheminlin266/deep-search-principles)

一个用于深度研究、行业分析、竞品调研和多源专业报告的通用 Agent Skill。

[English README](README.md)

## 功能

`deep-search-principles` 为 AI Agent 提供一套可复用的研究流程，重点包括：

- 为事实性主张绑定可追溯的 Markdown 引用
- 使用独立来源进行交叉验证
- 明确区分事实、估计、公司指引、市场共识和分析推断
- 检查来源时效性、出处和证据质量
- 执行查询扩展、四轮重试、搜索饱和度检查和覆盖跟踪
- 主动寻找反方观点、失败案例和风险证据
- 用证据账本和覆盖矩阵管理关键主张
- 防范网页、PDF 和搜索结果中的提示词注入

本技能提供研究规范，不提供搜索引擎、付费数据或固定来源清单。

## 安装

将本仓库发布到 GitHub 后，可通过开源 skills CLI 安装：

```bash
# 将 <owner>/<repo> 替换为公开 GitHub 仓库的所有者和仓库名。
npx skills add <owner>/<repo> --skill deep-search-principles

# 全局安装并跳过交互确认。
npx skills add <owner>/<repo> --skill deep-search-principles -g -y
```

也可以手动将 `SKILL.md` 放入所使用 Agent 支持的 skill 目录。

## 适用场景

适用于：

- 深度研究或综述类任务
- 行业、市场和竞品分析
- 产品、公司、技术或政策研究
- 需要近期、多源、可审计证据的专业报告

简单事实查询、随意头脑风暴，或不需要证据链的简短摘要通常不必使用本技能。

## 仓库结构

```text
.
├── SKILL.md             # 可安装的技能文件
├── README.md            # 英文文档
├── README.zh-CN.md      # 中文文档
├── LICENSE              # MIT 许可证
└── .gitignore
```

本仓库将 `SKILL.md` 放在根目录，因此可以被 skills CLI 识别为单技能仓库，也可以被 [skills.sh](https://skills.sh/) 索引。

## 兼容性

本技能遵循可移植的 `SKILL.md` 格式，不需要运行时依赖，可用于支持 skills 的 Agent，包括 Codex、Claude Code、Cursor、OpenCode 以及 skills CLI 支持的其他 Agent。

## 发布到 skills.sh

不需要单独上传或提交申请。发布流程是：

1. 保持仓库公开，并确保 `SKILL.md` 有效。
2. 分享安装命令：

   ```bash
   npx skills add zheminlin266/deep-search-principles
   ```

3. 等待安装量积累。[skills.sh](https://skills.sh/) 目录基于 skills CLI 的匿名使用数据生成；关闭遥测或在 CI 中完成的安装不会计入目录排名。

## 更新技能

编辑 `SKILL.md`，保持 YAML frontmatter 有效，然后将变更推送到 GitHub。GitHub 仓库是唯一事实来源，不需要额外生成安装包。

## 贡献

欢迎提交能提升证据可追溯性、来源严谨性或执行效率的改进。不要加入虚构的示例、URL、统计数字或事实性结论。

## 许可证

[MIT](LICENSE)
