# Ask Elon

Ask Elon 是一个通用的 [Agent Skill](https://agentskills.io/specification)，可以用中文和你聊天。它根据埃隆·马斯克的公开访谈，模拟他怎样看问题、做取舍和改变主意。即使你问“马斯克会怎么做？”，它也会用第一人称直接答你。它不是马斯克本人，回答也不是他的原话或背书。

本项目的主要参考资料是[向阳乔木（X：@vista8）](https://x.com/vista8)创建的[《马斯克全访谈》网站](https://elon.qiaomu.ai/)。主提示词和案例笔记都依据该站收录的访谈整理而成。

## 安装

如果你的 Agent 支持 Agent Skills，可以用 [Skills CLI](https://github.com/vercel-labs/skills) 安装。运行下面的命令，然后选择你使用的 Agent：

```sh
npx skills add yulizhou/ask-elon-skill
```

也可以手动安装：把仓库下载到你的 Agent 使用的 skills 目录，文件夹命名为 `ask-elon`，让 `SKILL.md` 和 `references/` 并排放在里面。

## 推荐用法：放进你的 Personal Agent

建议把 Ask Elon 放进你平时就会找它聊天的个人助手（Personal Agent）里，比如自己的 Grok Bot。这样你可以拿一个真实问题开聊，过几天再带着结果回来，看看新信息会不会让它改变判断。

如果你的 Bot 只支持自定义指令，可以把[主提示词](references/main-prompt.md)粘贴进去。这样就能开始聊；如果还希望它查到具体访谈，并且 Bot 支持上传参考文件，可以再附上[案例笔记](references/cases.md)和[访谈索引](references/episodes.tsv)。

安装好以后，可以直接这样问：

> 问问马斯克：我们做出了第一台样机。投资人想看第二台，我想先知道第一台到底贵在哪里。你会先干什么？

接下来可以补充数字、反驳它，或者问一句：“这是你在哪次访谈里说的？”

## 资料和许可

[案例笔记](references/cases.md)按主题整理了访谈里的例子和反例。[逐条索引](references/episodes.tsv)列出整理时收录的 651 个页面，其中 588 个有可读字幕，另 63 个仅登记目录。索引区分本人自述、采访者发言和第三方评论，也标记重传、模拟及归属不明的内容。

《马斯克全访谈》的原始访谈档案来自 [Elon Musk Archive](https://silicon-valley.tech/)。仓库只提供提示词、整理笔记、索引和出处链接，不附访谈全文或音视频。本项目与马斯克本人及其公司无隶属或合作关系。

本项目的原创内容使用 [MIT 许可证](LICENSE)。访谈、节目名称等第三方内容的权利仍归原权利人。
