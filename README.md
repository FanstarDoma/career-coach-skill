# 求职辅导 Skill

面向大学生的求职辅导 Skill：方向探索、准备规划与基于真实经历的简历修改。支持北美及海外商科求职，从你现在卡住的问题开始。

**当前版本：v0.5 试用版。** 已检查文件结构、引用和安装包完整性；尚未完成多客户端、跨岗位的真实使用验证，也没有招聘效果验证。

[下载 v0.5 安装包](https://github.com/FanstarDoma/career-coach-skill/releases/download/v0.5/career-coach-v0.5-install.zip) · [查看版本说明](https://github.com/FanstarDoma/career-coach-skill/releases/tag/v0.5) · [完整安装说明](求职辅导Skill-安装说明.txt) · [反馈问题](https://github.com/FanstarDoma/career-coach-skill/issues)

## 它能帮你做什么

| 你现在的情况 | 这版 Skill 会怎样帮助你 |
| --- | --- |
| 不知道选择什么方向 | 从真实经历和工作偏好出发，通常通过累计两三个关键问题，提出有依据、可调整的探索方向。 |
| 已有目标，不知道怎么准备 | 结合已有经历、申请时间和可投入时间，确定近期最重要的准备事项与完成标准。 |
| 正在准备申请 | 对照目标岗位判断哪些经历值得突出、哪些事实需要补充，再给出简历修改稿及关键取舍。 |

已经有明确问题时，直接处理，不要求先做性格测试或走完所有入口。没有正式实习或完整简历，也可以从课程、社团、兼职和个人项目开始。

## 两条核心做法

- **改写有依据。** 重要修改对应到你提供的事实，区分个人贡献、团队成果、计划和已完成工作。既不夸大经历，也不为了保守而删弱有依据的贡献。
- **缺口有行动。** 做过但没写清的，改写；信息不足的，只补问关键事实；确实没做过的，在有必要时提出一项能完成、可核实的准备行动。

重要简历修改会同时检查经历值得保留的理由，以及招聘方可能提出的合理质疑，最后落实到明确的选材或改写决定。这是辅助审查方法，不代表真实 recruiter 的独立评价或公司的内部评分模型。

## 安装

下载上方提供的 `career-coach-v0.5-install.zip`。它只包含完整的 `career-coach` Skill 文件夹和随包许可证；GitHub 自动生成的整个仓库源码 ZIP 具有不同目录结构。

### Claude 网页版或桌面版

在允许使用 Skills、已启用代码执行与文件创建的账户中，打开 **Customize → Skills → Create skill → Upload a skill**，上传安装 ZIP 并启用 `career-coach`。新开聊天后说“请使用 career-coach 求职辅导 Skill”，再提出自己的问题。

### Codex 本地环境

解压后，将整个 `career-coach` 文件夹放到 `~/.agents/skills/`，确保入口为 `~/.agents/skills/career-coach/SKILL.md`。也可以把安装包路径交给 Codex，让它安装；已有同名 Skill 时先比较，不直接覆盖。

新开聊天，在 Skill 选择器中选择“求职辅导”；Codex CLI／IDE 中可输入 `$career-coach`。如果尚未显示，重启客户端后检查。

### Claude Code 本地环境

解压后，将整个 `career-coach` 文件夹放到 `~/.claude/skills/`，新开会话后通过 `/career-coach` 调用。

其他工具需支持 Agent Skills，并按各自的安装规则导入。完整步骤、Windows／远程环境说明和故障处理见[安装说明](求职辅导Skill-安装说明.txt)。安装方式参考 [OpenAI Docs](https://learn.chatgpt.com/docs/build-skills)、[Claude 帮助中心](https://support.claude.com/en/articles/12512180-use-skills-in-claude)及 [Claude Code 文档](https://code.claude.com/docs/en/skills)。

## 安装后可以直接这样问

> 我大二，还不确定找什么方向。想从自己做过的事情开始，理清值得探索的工作。

> 我想申请商业分析实习，每周能准备 3 小时。帮我决定先做什么。

> 这是目标岗位和一段真实经历。请判断哪些内容值得突出、哪些信息需要补充，再帮我修改简历。

## 当前范围

- 当前重点是方向探索、岗位理解、准备规划和简历修改；面试辅导与申请跟踪尚待设计。
- 不编造用户量、收入、效率提升、个人职责或申请资格，不输出没有依据的匹配分数或录取保证。
- 当前岗位和项目状态需要官方信息核验；没有联网能力时，使用你提供的招聘说明，并保留未知项。
- 不含 coffee chat、联系人搜寻或自动投递流程。Skill 不包含回传反馈或上传简历的程序；所用 AI 平台的数据处理规则仍然适用。
- Skill 免费提供，不要求单独配置 API key；使用时仍依赖你所选 AI 工具的账户、额度和可用能力。

## 如何反馈

首次试用先完成一个真实任务。欢迎在 [Issues](https://github.com/FanstarDoma/career-coach-skill/issues) 中提供：

1. 使用的产品、模型（未知可注明）、Skill 版本及安装是否成功。
2. 你原本想解决的问题。
3. 哪段有用，哪里理解错了、追问太多或让你想退出。
4. 相关的少量输入与输出，尤其是事实被写错或真实贡献被删弱的地方。

提交前请去掉姓名、联系方式及不便公开的信息；不需要上传整份简历。反馈用于后续共同修改，这一版仍需要真实场景验证。

## 文件与许可

`career-coach/SKILL.md` 为入口；`references/` 保存招聘方视角的审查方法与示例；`agents/openai.yaml` 提供 Codex 显示信息。

采用 [MIT License](LICENSE)，版权声明为 Copyright (c) 2026 FanstarDoma。分发时保留许可证与版权声明。
