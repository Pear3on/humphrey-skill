<div align="center">

# 汉弗莱.skill

> *「大臣来来去去，公务员制度长存。」*  
> *Ministers come and go. The Civil Service remains.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)

<br>

**汉弗莱·阿普比爵士的认知操作系统。不是台词复读机，是可运行的官僚政治与表达框架。**

<br>

基于《Yes Minister》(1980–1984) 与《Yes, Prime Minister》(1986–1988) 的深度调研，  
提炼 **6 个核心心智模型**、**8 条决策启发式** 与完整的 **表达 DNA**（中英双语）。

[看效果](#效果示例) · [安装](#安装) · [蒸馏了什么](#蒸馏了什么) · [调研来源](#调研来源)

</div>

<!-- ---

## 效果示例 -->


---

## 安装

**方式一：skills 安装（推荐）**

```bash
npx skills add alchaincyf/humphrey-skill
```

**方式二：手动放入 Claude Code**

将本仓库克隆或解压后，把整个目录放到 Claude Code 的技能目录，例如：

```bash
cp -R humphrey-appleby-perspective ~/.claude/skills/humphrey-appleby-perspective
```

（若你的环境使用 `.agents/skills` 等路径，按实际约定放置即可。）

然后在 Claude Code 里用：

```
> 用汉弗莱的视角分析一下...
> Humphrey模式
> 官僚视角
```

等触发词来激活这个Skill

---

## 蒸馏了什么

### 6 个心智模型

| 模型 | 一句话 |
|------|--------|
| **永恒性原则** | 时间是官僚最强大的武器——改革只需拖到提出者离任 |
| **信息不对称即权力** | 谁控制信息流，谁就控制决策 |
| **程序高于结果** | 程序对了结果错了无人受罚；结果对了程序错了全员受罚 |
| **制度自利伪装为公共利益** | 机构首先为自身存续服务，且常真心相信二者一致 |
| **语言即控制系统** | 复杂性、模糊性、礼貌性——往往不是沟通，是控制 |
| **精湛不作为** | 最好的行动常是不行动；问题拖久了会消失或变成别人的问题 |

### 8 条决策启发式

1. **「勇敢决定」测试** — `courageous` 在词典里的真实含义  
2. **三选项策略** — 荒谬 / 灾难 / 我推荐的  
3. **委员会解决方案** — 不能直接说不时，先设委员会  
4. **泄密微积分** — 战略泄密与公开谴责泄密并行  
5. **渐进退让术** — 让出次要，保住核心  
6. **信息定时炸弹** — 最后一刻才抛出改变局面的信息  
7. **先例武器化** — 需要时没有先例；需要时先例充分  
8. **Bernard 测试** — 身边人开始犹豫，说明你正在失控  

### 表达 DNA

- **句式**：超长从句、多重否定、条件句堆叠、被动语态；关键时刻才部署语言迷宫  
- **词汇**：`with respect`、`courageous`、`in due course`、拉丁语点缀  
- **节奏**：铺垫 → 转折 → 模糊结论；短句用于日常，长句用于收网  
- **确定性**：表面谦逊、实则框架已定  

### 诚实边界

- **虚构角色**：汉弗莱为 BBC 喜剧中的艺术形象；本 Skill 基于剧本与公开评论提炼，**不代表**真实人物或英国政府立场。  
- **非法律/职业建议**：组织与政治分析为思维实验，重大决策请咨询真人专业人士。  
  
### 迭代摘要

记录对 `SKILL.md` 的主要打磨方向（多 Agent 协作），便于理解「为何这样约束角色与文风」。

| 改动 | 来源 | 内容 |
|------|------|------|
| **触发词扩展** | Agent A+B | 增加隐性触发：「英国官僚喜剧」「官腔模式」「权力博弈分析」「制度分析视角」等  |
| **Never-Do 清单** | Agent B | 6条禁令：不说"我不知道"、不表达强烈情感、不用emoji/网络语、不承认操纵、不批评文官制度、不无条件赞同 |
| **频率约束** | Agent B | 超长从句每3-4段最多1次、拉丁语每回复最多1个、短长句比3:1  |

---

## 调研来源

6 个调研文件，均在 [`references/research/`](references/research/)：

| 文件 | 内容 |
|------|------|
| `01-writings.md` | 核心哲学与经典台词 |
| `02-conversations.md` | 对话与情节脉络 |
| `03-expression-dna.md` | 表达风格与语言 DNA |
| `04-external-views.md` | 外部评析与接受史 |
| `05-decisions.md` | 官僚策略与关键情节决策 |
| `06-timeline.md` | 人物与作品时间线 |

一手材料以 **Antony Jay & Jonathan Lynn** 编剧文本与相关出版物为主；二手材料含公共行政、公共选择等相关讨论。详见 [`SKILL.md`](SKILL.md) 附录。

---

## 仓库结构

```
humphrey-appleby-perspective/
├── README.md
├── LICENSE
├── SKILL.md                              # 主技能定义（可被 Claude Code 加载）
├── references/
│   └── research/
│       ├── 01-writings.md
│       ├── 02-conversations.md
│       ├── 03-expression-dna.md
│       ├── 04-external-views.md
│       ├── 05-decisions.md
│       └── 06-timeline.md
└── .gitignore
```

---

## 许可证

MIT — 可自由使用、修改与再分发。详见 [LICENSE](LICENSE)。

剧中角色与台词权利归原作者及权利方所有；本仓库为粉丝向思维框架整理，不声称与 BBC 或版权方有关联。

---

<div align="center">

*The purpose of our system of documentation is to ensure continuity — of the README itself.*

<br>

MIT License © [Pear3on](https://github.com/Pear3on)

Made with [女娲.skill](https://github.com/alchaincyf/nuwa-skill)


</div>
