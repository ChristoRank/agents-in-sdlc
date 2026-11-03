---
slug: zh-cn/real-world-development/cli
title: "GitHub Copilot CLI"
description: "在学习 Copilot CLI 模式、自定义功能、MCP 工具和拉取请求自动化的同时，构建、验证并交付 Tailspin Toys 的两项更改。"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** 将 GitHub Copilot 作为代理式编码助手带入终端。它可以探索代码库、生成代码、运行命令，并连接外部工具——全部通过命令行完成，无需切换到图形化编辑器即可保持工作流畅。

本工作坊将带你完成 Tailspin Toys 中的一组连续任务。先在 GitHub Codespaces 中准备项目、安装 Copilot CLI 并熟悉其用法。然后添加星级评分，在浏览器中检查结果，并手动合并第一个拉取请求 (PR)。接下来从筛选 issue 入手，在 Plan 模式中确定方案，在 Autopilot 模式中实现，并在 Interactive 模式中审查。之后更新存储库指令、自定义 `quality-checks` 技能、使用 Playwright MCP 检查筛选功能，并创建 QA 智能体。最后审查完整更改，并使用 Agent Merge 合并筛选 PR。

你将创建两个 PR：一个用于星级评分，另一个用于筛选，并包含指令更新、技能更新、QA 配置和测试。筛选和质量工作流共用一个对话和分支，方便在学习各项工具时继续推进工作。你还可以学习[使用 GitHub Copilot CLI 和 Foundry 的可选系列课程][foundry]。

## 练习

| 练习 | 主题 | 说明 |
|----------|-------|-------------|
| [0. 先决条件][ex0] | 设置 | 创建存储库和 Codespace |
| [1. 安装 Copilot CLI][ex1] | 安装 | 安装并验证 Copilot CLI，然后熟悉其用法 |
| [2. 添加星级评分：快速改进][ex2] | 首次更改 | 显示现有评分和无评分时的备用值，然后合并第一个 PR |
| [3. 智能体模式：Plan 和 Autopilot][ex3] | 智能体模式 | 从 issue 规划功能，使用 Autopilot 构建，并在 Interactive 模式下审查 |
| [4. 使用自定义指令引导 Copilot][ex4] | 上下文 | 探索并更新指令，然后将其应用于筛选工作 |
| [5. 自定义并使用 quality-checks 技能][ex5] | 可重复的检查 | 探索现有技能、更改报告格式并运行技能 |
| [6. 使用 Playwright MCP 验证功能][ex6] | 浏览器观察 | 在 CLI 中配置 MCP 并检查筛选行为 |
| [7. 创建并使用 QA 智能体][ex7] | 需求和覆盖范围 | 创建并选择专用配置，然后收集最终验证证据 |
| [8. 创建并合并功能 PR][ex8] | 审查和合并 | 审查完整更改、创建 PR 并使用 Agent Merge |
| [9. GitHub Copilot CLI 中的斜杠命令][ex9] | CLI 功能 | 探索上下文、模型、共享，以及可选的云智能体委派 |
| [10. 总结和后续步骤][ex10] | 总结 | 回顾工作流、可复用的自定义功能和更多资源 |
| [可选：集成 Foundry][foundry] | 托管智能体 | 准备模型、构建并部署基于目录的 Backer Concierge，并将其连接到网站 |

## 先决条件

参加本工作坊前，请确保已具备以下条件：

- [ ] 拥有 GitHub 账户，并已启用 **Copilot Student、Pro、Pro+、Business 或 Enterprise** 计划
- [ ] 有权限创建存储库和 Codespace
- [ ] 基本了解终端或命令行操作

> [!TIP]
> 没有付费计划？已验证学生可通过 [GitHub Education][callout-student-plan-education] 免费使用 GitHub Copilot。**Copilot Student** 计划包含本工作坊所用的智能体、MCP、代码审查和 Copilot CLI 功能，因此可以完整完成所有路径。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> 如果使用的是 Copilot Business 或 Copilot Enterprise，请确认管理员已启用 Copilot CLI。

## 开始

**[从练习 0：先决条件开始 →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
