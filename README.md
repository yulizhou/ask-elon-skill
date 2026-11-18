# Ask Elon

一个用中文和你聊天的 Codex skill。它根据埃隆·马斯克的公开访谈，模拟他怎样看问题、做取舍和改变主意。即使你问“马斯克会怎么做？”，它也会用第一人称直接答你。它不是马斯克本人，回答也不是他的原话或背书。

本项目的主要参考资料是[向阳乔木（X：@vista8）](https://x.com/vista8)创建的[《马斯克全访谈》网站](https://elon.qiaomu.ai/)。主提示词和案例笔记都依据该站收录的访谈整理而成。

## 在 Codex 中使用

把仓库克隆到 Codex 的个人 skills 目录，然后打开一个新对话：

```sh
mkdir -p ~/.codex/skills
git clone https://github.com/yulizhou/ask-elon-skill.git ~/.codex/skills/ask-elon
```

在新对话里输入 `$ask-elon`，后面跟上问题。例如：

> $ask-elon 我们做出了第一台样机。投资人想看第二台，我想先知道第一台到底贵在哪里。你会先干什么？

你可以接着补充数字，反驳它，或换个话题闲聊。想核实历史说法时，可以直接问“这是哪次访谈里说的？”。

如果已经用 Git 安装过，在安装目录运行 `git pull --ff-only` 即可更新；如果之前手动复制过同名目录，请先备份，再选择是否替换。不用 Codex 时，也可以单独复制[主提示词](references/main-prompt.md)使用。

## 资料和许可

[案例笔记](references/cases.md)按主题整理了访谈里的例子和反例。[逐条索引](references/episodes.tsv)列出整理时收录的 651 个页面，其中 588 个有可读字幕，另 63 个仅登记目录。索引区分本人自述、采访者发言和第三方评论，也标记重传、模拟及归属不明的内容。

《马斯克全访谈》的原始访谈档案来自 [Elon Musk Archive](https://silicon-valley.tech/)。仓库只提供提示词、整理笔记、索引和出处链接，不附访谈全文或音视频。本项目与马斯克本人及其公司无隶属或合作关系。

本项目的原创内容使用 [MIT 许可证](LICENSE)。访谈、节目名称等第三方内容的权利仍归原权利人。
