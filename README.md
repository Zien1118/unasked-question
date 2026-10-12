# unasked-question

A Cursor Agent Skill that reads a long AI-coding conversation history and names the one deeper question the person kept circling but never asked. It is meant to be run again later: each pass sharpens, splits, or retires that question instead of inventing a new slogan.

给长期使用 AI Coding 的人。从他自己的 Cursor 对话里，找出一直在打转、却没有问出口的那一个问题。可以过一阵再跑一轮，用来避免项目一长就思维发乱、灵感接不上。

## 它交付什么

一句当事人认得出、并且会改变下一步决定的问题。加上这条问题被哪些表面讨论围着，以及问出口之后哪个决定会变。

它不交付聊天综述，也不把助手上次的结论改写成「你的核心问题」。

## 安装

把本仓库放到 Cursor 技能目录下，文件夹名保持 `unasked-question`，里面要有 `SKILL.md`。

个人技能，所有项目可用：

```text
%USERPROFILE%\.cursor\skills\unasked-question\
```

只在某一个项目里使用：

```text
<项目>\.cursor\skills\unasked-question\
```

新开一个对话后，技能会按描述里的触发条件被带起来。也可以直接说下面这些话。

## 怎样说会命中

这些说法和技能描述里的触发词一致，模型更容易把它读进来：

- 遍历我的对话，看有没有一个更深的问题我一直没问出口
- 这个长期项目我在打转，思维有点乱，灵感也接不上
- 按上一轮洞察再跑一轮，收紧或退役那个核心问题

目标已经明确的实现、修一个已知报错、问一次怎么操作，不会走这个技能。

## 循环记录

跑在某个长期项目上时，记录写在那个项目的 `insight-loop/LATEST.md`，不写回本仓库。下一轮先读这份记录。模板在 `templates/loop-record.md`。

记录里不要留下密钥、令牌和密码。对话里如果出现过，引用时改成不含秘密的原意。

## 许可

MIT，见 [LICENSE](LICENSE)。
