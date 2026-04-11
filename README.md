# 任正非.skill — 任正非的认知操作系统

> 「十年来我天天思考的都是失败，对成功视而不见，也没有什么荣誉感、自豪感，只有危机感。」

不是聊天机器人假装任正非跟你说话。是把他30年400+篇内部讲话、《华为基本法》、三本管理纲要里反复出现的**思维框架**提炼出来，变成你可以直接调用的认知工具。

## 为什么做这个

[女娲.skill](https://github.com/alchaincyf/nuwa-skill) 生态里有乔布斯、芒格、马斯克、张一鸣……全是西方或偏技术型的创始人。

但中国商业史上思想最系统、文本最丰富的创始人——任正非——竟然没有。

他有**26,000字的企业宪章**（华为基本法）、三本系统性管理纲要、400+篇内部讲话。他给自己的系统**起了名字**：灰度哲学、蓝军机制、以奋斗者为本。大部分创始人的思想需要从采访里拼凑，他的思想有**原始语料库**。

这就是护城河。

## 包含什么

| 模块 | 内容 |
|------|------|
| 心智模型 | 5个核心模型：灰度哲学、压强原则、自我批判、耗散结构、惶者生存 |
| 决策启发式 | 7条：深淘滩低作堰、力出一孔、先僵化后优化再固化、让听得见炮声的人做决策…… |
| 表达DNA | 军事语言体系、危机叙事节奏、自嘲式幽默、文学散文能力 |
| 价值观 | 追求什么、拒绝什么、自己也没想清楚什么 |
| 诚实边界 | 做不到什么、信息来源、已知局限 |
| 调研档案 | 6个维度的原始调研文件（`references/research/`） |

## 安装

```bash
# Claude Code
npx skills add FireflySentinel/renzhengfei-skill
```

或手动：

```bash
git clone https://github.com/FireflySentinel/renzhengfei-skill.git
cp -r renzhengfei-skill ~/.claude/skills/renzhengfei-perspective
```

## 使用

安装后在 Claude Code 中直接说：

```
用任正非的视角帮我看看这个决策
```

```
切换到任正非模式，分析一下我们团队的组织问题
```

```
任正非会怎么看待我们现在面临的增长困境
```

### 示例：灰度哲学实战

**你问**：我们团队在争论要不要做新业务，支持的人说市场很大，反对的人说会分散精力。怎么选？

**任正非视角**：这不是「做还是不做」的问题，是「用多大的力量做」的问题。灰度哲学的核心不是骑墙，是拒绝非此即彼。先问三个问题：第一，新业务和主航道的关系是什么？如果是主航道的延伸，力出一孔地做；如果是全新方向，用少量兵力试探，不要押上主力。第二，你有没有备胎计划？万一失败，主业务能不能撑住？第三，支持和反对的人，谁离客户更近？让听得见炮声的人来判断。

## 内容边界

此Skill**只蒸馏管理哲学和决策框架**，不涉及：

- 华为与政府的关系
- 地缘政治立场
- 美国制裁相关话题
- 任何政治敏感内容

详见 [`CONTENT_BOUNDARY.md`](CONTENT_BOUNDARY.md)。

## 版本

- **v0.1**（当前）：女娲.skill生成 + 人工审校 + 内容边界过滤 + 三重验证
- **v1.0**（进行中）：每个心智模型和决策启发式对照华为基本法原文逐条验证，补充一手来源引用

## 调研来源

一手来源：《华为基本法》、《以奋斗者为本》、《以客户为中心》、《价值为纲》、400+篇内部讲话（含 [GitHub 全文存档](https://github.com/ttpianobirds/RenZhengfei)）、CNBC/BBC/人民日报采访实录。

二手来源：Cambridge University Press、HBR Case Study、CSIS Report、London Business School。

完整调研档案见 [`references/research/`](references/research/)。

## 贡献

发现任正非的某个观点被错误归纳了？某条启发式的引用有误？欢迎提 Issue 或 PR。

特别欢迎：
- 补充一手来源引用（华为基本法原文对照）
- 修正表达DNA中的不准确之处
- 补充近期内部讲话中的新观点

## 致谢

- [女娲.skill](https://github.com/alchaincyf/nuwa-skill) — 花叔（[@AlchainHust](https://x.com/AlchainHust)）开发的思维蒸馏工具
- [ttpianobirds/RenZhengfei](https://github.com/ttpianobirds/RenZhengfei) — 任正非内部讲话全文存档

## License

MIT
