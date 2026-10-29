# 参考来源

本生成器将项目背景澄清、视觉方向、交互、动效、图片与验收方法组织为一套自包含流程。参考来源供了解设计依据，不是安装依赖。

## 按任务类型读取

- [操作型：工作台、后台与工具](../skills/project-design-skill-builder/references/operate-design-patterns.md)：任务流、表格、复杂表单、状态和恢复；参考 Carbon 表格与 Ant Design 表单的一手文档。
- [说服型：官网与产品展示](../skills/project-design-skill-builder/references/platform-design-patterns.md)：价值、证据、能力探索和下一步操作。
- [阅读型：文档、知识库与长文](../skills/project-design-skill-builder/references/read-design-patterns.md)：查找、理解、内容类型和阅读连续性；参考 Diataxis 与 W3C WAI 的内容组织和可访问结构方法。
- [体验型：作品集、展览与叙事](../skills/project-design-skill-builder/references/experience-design-patterns.md)：内容关系、叙事、媒体、探索和访客控制；结合 W3C WAI 的动效替代与播放控制说明。

操作型、阅读型和体验型参考为方法整理，不声称完成了真实后台、知识库或展览网站的案例审计。各文档末尾列出可选的一手来源；项目保留自己的设计系统，无需安装来源中的组件库。选中的方法会写进生成的项目 Skill。

## 交互、布局与主题

- [交互与布局方法](../skills/project-design-skill-builder/references/interaction-layout.md)：从 GOV.UK 用户需求与按钮规则、USWDS 设计原则、NN/g 的层级 / 渐进披露 / 可用性启发式 / 点击数研究，以及 W3C WAI 表单反馈中整理可执行方法。文档保留八个原始来源、项目改编与适用边界，最后核对于 2026-10-29。
- [主题与配色方法](../skills/project-design-skill-builder/references/color-direction.md)：按用户、场景、任务和品牌证据决定颜色角色，检查完整主题，避免固定奶白底或另一套通用配色。这是项目选色方法，不是调色板清单。

## 其他来源

- [Impeccable](https://impeccable.style/)：设计判断、反模板化检查与以具体任务组织能力。
- [Emil Kowalski](https://emilkowal.ski/)：操作反馈、过渡与界面细节。
- [千问开放平台](https://open.qianwen.com/) / [ByteDance Seed](https://seed.bytedance.com/zh/) / [火山引擎](https://www.volcengine.com/)：实际官网的视觉与信息层级观察。
- 更完整的观察及访问限制见 [source-notes.md](../skills/project-design-skill-builder/references/source-notes.md) 和 [official-site-observations.md](../skills/project-design-skill-builder/references/official-site-observations.md)。

安装命令采用 [Vercel Skills CLI](https://github.com/vercel-labs/skills)。仓库中的 Skill 可以从 GitHub 安装，不需要单独发布 npm 包。
