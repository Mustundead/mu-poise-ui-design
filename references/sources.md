# 资料与取舍

这是 MU LABS 的实践方法，不是 Apple 的官方设计标准。新写的指令与教学情境使用仓库 MIT 许可证；外部资料不因被链接而重新授权。本仓库不包含演讲逐字稿、第三方图像或来源不明的代码。

| 资料 | 解决的问题 | 采用与未采用 |
| --- | --- | --- |
| [Designing Fluid Interfaces · WWDC18](https://developer.apple.com/videos/play/wwdc2018/803/) | 输入与运动如何连接 | 采用及时反馈、连续接管和可打断的交互思路；不将演讲中的具体实现或参数宣称为所有平台的标准。 |
| [Apple HIG: Motion](https://developer.apple.com/design/human-interface-guidelines/motion) | 动效的目的和平台适配 | 作为当前原生设计查询入口；不据此规定所有界面都使用弹簧、玻璃或同一时长。 |
| [MDN: Pointer events](https://developer.mozilla.org/en-US/docs/Web/API/Pointer_events) | Web 指针捕获、取消和浏览器行为 | 用于核对生命周期与输入能力；不把触屏行为直接套在键盘和鼠标上。 |
| [W3C WAI: Dialog pattern](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/) | Web 模态焦点与退出 | 定向验证真正的模态；不把非模态面板强行做成模态。 |
| [MDN: prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion) | 运动偏好响应 | 保留任务反馈，调整相关效果；不只写一条会破坏状态机的全局 CSS。 |

2026-09-22 核对了 WWDC18 和 MDN Pointer events 页面；HIG Motion 页可访问，但其正文依赖页面运行环境，具体系统版本仍应按需查证。其他链接为问题导向的后续入口。

旧个人工作流名 `apple-design` 仅用于迁移定位。本版重新编写了结构、例子和实现边界：移除未有充分来源支持的年份归因、通用“Apple 参数”、强制模糊动画及“CSS 一律不可中断”等绝对化说法。平台名称不表示官方关联或背书。
