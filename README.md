# unasked-question

找出长期 AI Coding 项目里，反复讨论却从未问出口的那一个问题。下一轮只把这一句收紧、拆开或退役，不另发明一句口号。

Finds the one question a long AI-coding project kept circling but never asked, then sharpens or retires it on the next pass.

## 安装

仓库分支是 `master`。

```text
git clone -b master https://github.com/Zien1118/unasked-question.git
```

Cursor，所有项目可用：

```text
%USERPROFILE%\.cursor\skills\unasked-question\
```

Codex，所有项目可用：

```text
%USERPROFILE%\.codex\skills\unasked-question\
```

把克隆下来的仓库放进上面其中一个目录，目录名保持 `unasked-question`，里面要有 `SKILL.md`。只在某一个项目里使用时，改放到该项目的 `.cursor/skills/unasked-question\` 或 `.codex/skills/unasked-question\`。

## 支持范围

能读到的本机历史取决于当时的客户端和权限。读不到时，把相关原话粘贴进来，或提供你自己导出的记录。技能不会把没读到的部分说成已经看过。

会进入这个技能的说法：

- 遍历我的对话，看有没有一个更深的问题我一直没问出口
- 这个长期项目我在打转，思维有点乱，灵感也接不上
- 按上一轮洞察再跑一轮，收紧或退役那个核心问题
- Review my past chats and name the question I never actually asked
- I'm going in circles. Rerun the insight loop and tighten the last question

目标已经明确的实现、修一个已知报错、问一次怎么操作，不会走这个技能。

## 匿名演示

输入是三个月里的两类原话：「A 框架和 B 框架哪个先做？」以及「演示过了他们还是不会改。」没有人写下决定。

洞察：

还没问出口的那一句是「第一次成功之后，用户必须自己能改哪一件事？」

事实是选型和对演示的不满来回出现。判断是选型在给「能改哪一件事」收集材料。问出口之后，第一版只保留这一条路径，不再按演示覆盖面选框架。状态是新发现。

## 记录

跑在某个项目上时，当前指针是该项目的 `insight-loop/LATEST.md`。每一轮另存 `insight-loop/history/<时间戳>-<轮次ID>.md`。两份都只含脱敏摘要，不上传原始对话。

模板在 `templates/loop-record.md`。

## 许可

MIT，见 [LICENSE](LICENSE)。
