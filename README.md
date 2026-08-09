# 中文写作 AI 痕迹去除

一份针对中文写作的极简规则清单。把它交给 Agent，让 Agent 在写作或润色时识别并删掉常见的 AI 腔。

## 用法

打开 [`AI 味儿.md`](./AI%20味儿.md)，将下面这句与文件内容一起放进指令文件：

> 写作或润色中文时，检查并去除以下 AI 痕迹，保持表达自然、直接、简洁。

- Codex：单个项目使用项目根目录下的 `AGENTS.md`，全局使用 `~/.codex/AGENTS.md`。
- Claude Code：单个项目使用项目根目录下的 `CLAUDE.md`，全局使用 `~/.claude/CLAUDE.md`。

如果已有指令文件，直接追加即可。具体加载方式可查看 [Codex 官方文档](https://learn.chatgpt.com/docs/agent-configuration/agents-md) 和 [Claude Code 官方文档](https://code.claude.com/docs/zh-CN/memory)。

## 设计原则

提示词也有成本。规则越短，占用的 token 越少，也越容易维护。这个项目只保留能稳定复现、能直接改写的特征，用尽可能少的文字改善中文表达。

## 效果边界

这些规则用于减少常见的中文 AI 腔。项目不提供 AI 检测功能，也不保证绕过检测工具。

## 贡献

发现新的稳定特征时，欢迎提交 Issue 或 PR，并附上原句和更自然的改法。

## 许可

作者：Awesome-GitHub（[@Wechat-ggGitHub](https://github.com/Wechat-ggGitHub)）。

项目内容使用 [Creative Commons Attribution 4.0 International](./LICENSE) 许可。复制、修改或发布时，请保留署名并链接本仓库。
