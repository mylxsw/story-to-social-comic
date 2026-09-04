# Story to Social Comic

把故事、文章或观点改编成连续竖版漫画，并生成适合小红书和抖音的标题、正文与 Tags。

这个 Skill 不会机械地逐段配图。它会先理解原文，再重组视觉叙事、主动推荐漫画风格、建立角色与视觉设定、输出完整分镜，最后按“生成第一张”“下一张”的方式连续生成。

## 能做什么

- 提炼主题、冲突、人物关系、情绪曲线、金句和传播钩子；
- 主动提供 3–5 个适合当前内容的漫画风格选项，并标出推荐项；
- 规划约 6–10 张竖版漫画及完整逐页分镜；
- 建立 Character Bible 和 Visual Bible，保持人物、服装、道具与画风连续；
- 支持“生成第一张”“下一张”“重做这一张”的连续创作；
- 分别生成小红书与抖音标题、正文和 Tags；
- 区分事实、观点、比喻与非规范术语，避免虚假权威表达。

适用于心理故事、人生感悟、职场故事、历史故事、公众号文章和观点内容。它不用于普通知识卡片或单张无连续性的插画。

## 安装

在 Codex 中直接提出：

```text
帮我安装这个 Skill：https://github.com/mylxsw/story-to-social-comic
```

也可以克隆到 Codex Skills 目录：

```bash
git clone https://github.com/mylxsw/story-to-social-comic.git ~/.codex/skills/story-to-social-comic
```

安装后如未立即出现在技能列表中，请重新打开或新建任务以刷新技能索引。

## 使用

```text
使用 $story-to-social-comic 处理这篇文章：<粘贴文章或提供文件>
```

Skill 会先根据内容推荐漫画风格。选择风格后，它会输出内容分析、Character Bible、Visual Bible 和完整分镜。

之后可以连续输入：

```text
生成第一张
下一张
重做这一张：人物表情更紧张，其他设定不变
生成小红书和抖音发布文案
```

## 默认工作流

1. 理解原文并识别事实风险；
2. 推荐漫画风格，等待用户选择；
3. 完成漫画化重构与完整分镜；
4. 建立并锁定 Character Bible 和 Visual Bible；
5. 逐张生成并检查连续性；
6. 生成小红书和抖音发布素材。

详细行为、输出模板和质量标准见 [SKILL.md](SKILL.md)。
