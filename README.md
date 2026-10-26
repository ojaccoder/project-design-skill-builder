# Design Skill Builder

**为你的项目，生成一套设计规则。**

分析现有项目，问清用户、任务和设计偏好，将布局、文案、图片与动效要求整理成项目专属 Skill。新增页面或改版时，沿用同一套规则。

[官网](https://design-skill-builder.vercel.app) · [使用文档](https://design-skill-builder.vercel.app/docs.html)

## 安装

在项目目录运行，按提示选择你使用的编程助手：

```bash
npx skills add ojaccoder/project-design-skill-builder
```

需要 Node.js 22.20 或更新版本。默认安装到当前项目；希望多个项目都能使用时，在命令末尾加 `-g`。已安装的用户可运行 `npx skills check` 检查更新。

## 开始使用

在编程助手中打开项目，发送：

```text
使用 project-design-skill-builder 分析这个项目。
先问我影响设计的关键背景问题，再生成一套项目专属的设计 Skill。
重点去掉模板感和多余文案，明确图片与交互动效怎么用。
```

确认生成的规则后，再发送：

```text
按刚生成的项目设计 Skill 改造官网。
把图片和交互动效实际用起来，提供桌面、手机截图和交互录屏。
```

## 它解决什么

| 常见问题 | 生成的规则会明确什么 |
| --- | --- |
| 页面缺少重点：内容等重、布局重复、装饰与任务无关 | 谁在用、先看什么、先做什么，以及适合内容的视觉方向 |
| 文案空泛、标签太多，用户看不出重点 | 标题说具体用途，按钮说实际动作，状态说发生了什么；删掉口号、重复说明和装饰性标签 |
| 每次改页面都要重新解释审美 | 将布局、字体、颜色、图片方向和交互约定保存在项目中 |
| 图片和动效只是摆设 | 明确图片的内容用途、动效的触发与反馈、实现方式和验收条件 |

**Avoid unnecessary secondary labels and descriptions. Let the layout do the explaining.**

保留用户完成任务需要的信息：操作名称、错误原因和重要限制。简洁不等于把必要说明都删掉。

## 你会得到什么

一份项目专属 `SKILL.md`，以及按需要生成的视觉、交互、图片和验收参考文档。它们包含实际项目的用户、任务、约束和设计决定，后续新增页面与改版可以直接读取。

生成器负责制定规则。网页实现、生图和录屏由编程助手执行；图片模型、浏览器与录屏能力取决于助手环境。生成的文件保存在项目中，后续开发可以直接读取。

## 什么时候用

适合已有项目需要重新整理设计方向，或团队想把反复沟通的要求沉淀下来。已有清晰、可执行的设计规范时，可以直接沿用现有规范。结果仍需结合真实页面验证，不承诺一次生成就消除所有设计问题。

[界面文案规则](skills/project-design-skill-builder/references/interface-copy.md) · [详细使用方法](docs/getting-started.md) · [查看生成器](skills/project-design-skill-builder/SKILL.md)
