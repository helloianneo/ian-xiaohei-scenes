# Ian Xiaohei Scenes

Generate Chinese Xiaohei 2.0 illustrations:

```text
Xiaohei + real objects + physical action + whitespace narrative
```

This skill turns article ideas, user situations, project stories, and personal timelines into high-quality visual prompts for Xiaohei-style images.

## Modes

### Standard Mode

Use for 16:9 article illustrations.

- Pure `#FFFFFF` white background
- One real-object scene
- One Xiaohei physical action
- 2-4 short handwritten Chinese labels
- Sparse colored tape / dot accents
- Template masters:
  - `assets/examples/01-meeting-pull-in.png`
  - `assets/examples/02-message-overload.png`
  - `assets/examples/03-production-alert.png`
  - `assets/examples/04-code-review-rework.png`
  - `assets/examples/05-ai-automation-badge.png`
  - `assets/examples/06-ai-resume-filter.png`

### Long-Scroll Bonus Mode

Use when the request mentions:

```text
彩蛋模式 / 长卷故事图 / 超横版 / 个人经历 / 项目复盘 / 产品演化 / 成长路径
```

- Ultra-wide long-scroll story image
- Premium near-white background
- One winding hand-drawn route
- 5-8 real-object milestone nodes
- Xiaohei participates at every node
- Left opening, right closing
- Template master: `assets/examples/07-long-scroll-story-master.png`

## Usage

Invoke the skill with a topic, draft, article section, project story, or timeline nodes.

Examples:

```text
用 $ian-xiaohei-scenes 给这篇文章生成 4 张正文配图。
```

```text
用 $ian-xiaohei-scenes 的彩蛋模式，把这个项目复盘做成一张长卷故事图。
```

## Files

- `SKILL.md` - main workflow and routing rules
- `references/style-dna.md` - visual DNA and mode standards
- `references/story-extraction.md` - how to extract situations and timeline nodes
- `references/object-patterns.md` - real-object metaphor patterns
- `references/master-selection.md` - standard-mode master selection and delivery blocking rules
- `references/prompt-template.md` - generation prompt templates
- `references/qa-checklist.md` - quality gates and iteration rules
- `references/xiaohei-ip.md` - Xiaohei IP shape and behavior rules
- `assets/examples/` - template masters and quality references

## Open Source Note

- This installable skill directory is distributed under the repository license.
- `assets/examples/07-long-scroll-story-master.png` is the canonical long-scroll design master. It intentionally contains Ian-specific sample story labels and third-party brand references to preserve the quality bar; downstream users should treat them as template content, not default facts to copy.
