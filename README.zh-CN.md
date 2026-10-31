# Show the Change｜AI 改动看明白

**“AI 说已经做完了，我到底该看哪里？”**

一个给 Agent 用的小 Skill：把指定项目的改动讲成人能直接行动的话——你能看到什么、去哪里检查、还有什么没验证。适合使用编程 Agent、但不想先读一大页代码差异的人。

[English](README.md) · [查看 Skill 原文](skills/show-the-change/SKILL.md) · [看真实产品改动示例](examples/carousel-product-change.zh-CN.md)

## Agent 做完后，问一句

> “用 Show the Change 告诉我这次改了什么，我该怎么检查？”

Skill 引导 Agent 查看实际改动，用你的语言解释，并指出相应页面或文件。源码里写了什么，不等于网站已经更新，也不等于安装在电脑里的软件已经更新。

## 在 Codex 中安装

在需要使用它的项目目录，使用 Node.js 22.20 或更高版本运行：

```bash
npx skills@1.7.4 add LydiaTools/show-the-change --skill show-the-change --agent codex
```

然后说：**“用 $show-the-change 讲讲这个项目最近改了什么，告诉我去哪里检查。”**

这条命令使用可选的第三方安装器，可能下载代码。Skill 本身是一份指令，使用你已有的 Agent，不附带模型；Agent 原有的模型使用条件和费用仍适用。它不会安装 Git 钩子、阻止推送、发布项目或独立确认部署。

也可以手动把完整的 [`skills/show-the-change`](skills/show-the-change/) 文件夹复制到所用 Agent 支持的技能目录。如果该 Agent 的说明要求重启或重新加载，请照做。

## 一个真实改动示例

[产品示例](examples/carousel-product-change.zh-CN.md)解释了一次真实的图片工具改动，展示实际界面，并告诉你如何试用。[另一个示例](examples/browser-agent-doc-change.zh-CN.md)把文档更新和产品功能更新区分开。两份示例都基于公开源码和已有检查记录，不是独立的模型行为评测。

> **你能看到什么变化：** 横图、方图、竖图可以放进同一画幅，完整显示图片边缘；调整顺序后，可以一次下载带编号的压缩包。

![实际图片工具界面：三张不同形状的照片完整放在同一画幅中](https://raw.githubusercontent.com/LydiaTools/aspectory/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/carousel-photos-zh.jpg)

*截图是示例所介绍的现有 Aspectory 产品，不是本 Skill 的操作界面。图片使用分别署名的 CC0 练习照片；[查看来源](https://github.com/LydiaTools/aspectory/blob/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/PROVENANCE.md)。产品示例在当前源码中，较早的 v0.1.0 预览 ZIP 不包含。*

## 能做什么

- 引导 Agent 检查指定的差异、工作区状态或用户提供的文件，并给出相关依据。
- 区分预期效果与已经执行的测试、源码与已部署页面、未跟踪文件与已提交改动。
- 给出具体检查方法；不能保证解释绝对正确，不能证明软件安全，也不能替代代码审查或真实验收。
- 尚未对不同 Agent 或真实用户做系统评估。重要结果仍需在实际应用中确认。

思路受到公开讨论启发：[Sphinx](https://news.ycombinator.com/item?id=50137950) 在推送前向开发者提问，[Farol](https://news.ycombinator.com/item?id=50231349) 帮审查者寻找值得关注的改动。Show the Change 是独立编写的解释流程，未包含这两个项目的代码，也不代表获得它们的认可。

## 许可证

MIT。欢迎反馈问题或提交改进。
