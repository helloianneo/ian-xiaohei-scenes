# Ian Xiaohei Scenes

> 把中文内容里的处境、压力、转折和项目故事，变成“小黑 + 真实物件 + 物理动作 + 留白叙事”的正文配图。
>
> 16:9 正文图 | 彩蛋长卷故事图 | 真实物件小现场 | 小黑 IP | Codex Skill

---

## 这个仓库是什么

Ian Xiaohei Scenes 是一个 Codex Skill，用来指导 AI Agent 为中文文章、帖子、教程、案例、项目复盘和个人经历生成“小黑 2.0”视觉配图。

它不是通用插画 prompt，也不是 PPT 信息图模板。它的核心目标是：先理解内容里的真实处境，再把其中一个抽象判断变成一个可看见的物理现场。

核心公式：

```text
小黑 + 真实物件 + 物理动作 + 短中文标签 + 留白叙事
```

一句话：**让读者先看到一个真实、轻、怪的小现场，再在 1 秒内意识到“这说的就是我”。**

---

## 和 1.0 的区别

[Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) 是 1.0：更像白板上的手绘解释图，适合拆观点、拆流程、拆方法。

Ian Xiaohei Scenes 是 2.0：更像白色摄影棚里的真实物件现场，适合表达处境、情绪、项目故事、产品演化和正文观点隐喻。

| 版本 | 视觉核心 | 适合内容 |
| --- | --- | --- |
| 1.0 Illustrations | 纯白手绘解释图 | 方法论、流程、结构、认知拆解 |
| 2.0 Scenes | 真实物件小现场 | 用户处境、工作压力、AI 时代状态、项目复盘、个人经历 |

---

## 两种模式

### 标准模式

用于 16:9 正文配图。

- 纯白色背景
- 一个真实物件小现场
- 一个核心物理动作
- 小黑必须承担动作
- 2-4 个中文短标签
- 少量蓝 / 粉 / 黄 / 绿 / 红点缀

### 彩蛋长卷模式

用于个人经历、项目复盘、产品演化和成长路径。

- 超横版长卷故事图
- 高级近白背景
- 一条手绘曲线路径
- 5-8 个真实物件节点
- 每个节点都有小黑参与动作
- 左侧起点，右侧收束
- 不做编号时间轴，不做 PPT 流程图

---

## 适合谁用

特别适合：

- 写中文文章，需要正文配图的人
- 做 AI 工作流、产品复盘、个人经历、项目故事的人
- 想把“打工人处境”“AI 时代焦虑”“创作者卡点”画出来的人
- 想要比 PPT 信息图更轻、更怪、更有个人识别度的配图风格的人
- 用 Codex 做内容生产，希望稳定复用一套视觉语言的人

不适合：

- 想要商业 KV、品牌海报或精致扁平插画的人
- 想要传统流程图、复杂架构图、课程课件的人
- 想要聊天 UI、App 截图、仪表盘截图的人
- 想把大量正文、长段解释或完整流程塞进一张图里的人
- 需要严格可编辑矢量源文件的人

---

## 示例效果

下面 7 张图是本 Skill 的高质量模板母版和风格标尺。它们不是死板模板；使用时应该学习比例、留白、真实物件质感、小黑动作和叙事关系，不要机械复刻物件组合和构图。

### 会议拉回

![会议拉回](examples/images/01-meeting-pull-in.png)

### 消息过载

![消息过载](examples/images/02-message-overload.png)

### 生产报警

![生产报警](examples/images/03-production-alert.png)

### 审查返工

![审查返工](examples/images/04-code-review-rework.png)

### AI 自动化身份重命名

![AI 自动化身份重命名](examples/images/05-ai-automation-badge.png)

### AI 简历筛选

![AI 简历筛选](examples/images/06-ai-resume-filter.png)

### 彩蛋长卷故事图

![彩蛋长卷故事图](examples/images/07-long-scroll-story-master.png)

---

## 安装

克隆仓库：

```bash
git clone https://github.com/helloianneo/ian-xiaohei-scenes.git
cd ian-xiaohei-scenes
```

复制 skill 到 Codex skills 目录：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./ian-xiaohei-scenes "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 里使用：

```text
Use $ian-xiaohei-scenes 为这篇中文文章设计并生成几张小黑实物场景正文配图。
```

---

## 怎么用

### 只做配图规划

```text
Use $ian-xiaohei-scenes 先不要生图。
请分析下面这篇文章哪里适合做“小黑 + 真实物件 + 物理动作”的正文配图。
输出 5 张左右的 shot list。

<粘贴文章>
```

### 直接生成正文配图

```text
Use $ian-xiaohei-scenes 把下面这篇文章生成 4 张小黑实物场景正文配图。
要求：16:9 横版、纯白背景、真实物件、小黑参与核心动作、2-4 个中文短标签。

<粘贴文章>
```

### 彩蛋模式长卷

```text
Use $ian-xiaohei-scenes 的彩蛋模式，把这个项目复盘做成一张超横版小黑长卷故事图。
```

更多示例见 [examples/prompts.md](examples/prompts.md)。

---

## 工作流程

这个 skill 的流程是：

1. 读取文章、主题、项目经历或时间线节点
2. 提炼读者处境、核心冲突和适合视觉化的物理动作
3. 标准模式先从 01-06 中锁定一张母版；彩蛋模式锁定 07 长卷母版
4. 写出母版不变量、当前内容变异点、3 秒读懂句和失败信号
5. 选择一个真实主物件或紧凑主物件组
6. 让小黑承担核心物理动作
7. 每张图单独调用图像模型生成
8. 按 QA checklist 检查：比例、留白、真实物件、小黑动作、中文标签、非 PPT 感、非母版复刻
9. 保存最终 PNG，并报告用途和路径

---

## 目录结构

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── ian-wechat-qr.jpg
├── examples/
│   ├── images/
│   │   ├── 01-meeting-pull-in.png
│   │   ├── 02-message-overload.png
│   │   └── ...
│   └── prompts.md
└── ian-xiaohei-scenes/
    ├── SKILL.md
    ├── README.md
    ├── agents/
    │   └── openai.yaml
    ├── assets/
    │   └── examples/
    └── references/
        ├── style-dna.md
        ├── xiaohei-ip.md
        ├── story-extraction.md
        ├── object-patterns.md
        ├── master-selection.md
        ├── prompt-template.md
        └── qa-checklist.md
```

真正需要安装到 Codex 的是子目录：

```text
ian-xiaohei-scenes/
```

根目录的 README、LICENSE、NOTICE 和 examples 是 GitHub 分享文档。

---

## 注意事项

- 每张标准图只讲一个核心物理动作。
- 图片里的中文文字越短越稳定。
- 小黑必须承担核心动作；如果去掉小黑画面仍然完全成立，说明小黑太装饰了。
- 示例图是质量母版，不是可描摹模板。
- 彩蛋长卷里的个人经历节点可以保留作为风格锚点；生成新图时应替换成当前用户自己的事实和节点。
- AI 图像模型可能出现错字、幻觉标签、风格漂移或多余标题，生成后需要检查。
- 如果中文错字严重，优先减少标注词并重生成。

---

## 相关项目

- [Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) - 中文小黑手绘正文配图 1.0
- [Ian Handdrawn PPT](https://github.com/helloianneo/ian-handdrawn-ppt) - 中文手绘技术 PPT-style 页面图生成 Skill
- [Awesome Claude Code Skills](https://github.com/helloianneo/awesome-claude-code-skills) - Claude Code Skills / Agents / Plugins 精选合集
- [Obsidian + Claude AI Second Brain](https://github.com/helloianneo/obsidian-ai-second-brain) - Obsidian + Claude AI 个人知识库搭建指南

---

## 关于作者

**Ian (伊恩)** — 产品设计师 / 一人公司实践者 / AI Builder

用 AI 团队打造一人公司。

- GitHub: [helloianneo](https://github.com/helloianneo)
- X/Twitter: [@ianneo_ai](https://x.com/ianneo_ai)
- 网站: [www.ianneo.xyz](https://www.ianneo.xyz)
- 微信: `ianneoxyz`
- 邮箱: hello.neoc@gmail.com

---

## 继续探索

这套小黑实物场景图 Skill，只是我用 AI 搭建个人生产系统里的一个小工具。

如果你也在用 AI 做内容、知识库、工作流或产品化，可以继续看我的网站：[www.ianneo.xyz](https://www.ianneo.xyz)。

只想先观察，可以关注我的 [X/Twitter](https://x.com/ianneo_ai)。

想了解 Indie Builders Club，加微信：`ianneoxyz`，备注「OPC」。

<p>
  <img src="assets/ian-wechat-qr.jpg" alt="Ian 微信二维码" width="120">
</p>

不方便扫码也可以搜索微信：`ianneoxyz`。

---

## License

MIT License. See [LICENSE](LICENSE).
