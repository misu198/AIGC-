# Midjourney 高级 Prompts-重混 Remix

---

使用 Remix 模式来在变化(V)之间更换 Prompts、参数、模型版本或纵横比。Remix会将您的起始图像的整体构成作为新的任务的一部分。Remix 可以帮助改变图像的设置或照明、衍变题材或实现复杂的组合。



`Remix` 是一项实验性功能，可能随时更改或删除。



## 使用Remix

要使用Remix,请使用 `/prefer remix` 命令或使用 `/settings` 命令并切换 `🎛️ Remix` 模式按钮来激活 Remix模式。启用 Remix 后，变化按钮（V1、V2、V3、V4）在图像网格下默认交互会改变。当启用 Remix 时，它允许您（弹窗）在每个变体中编辑您的 Prompts。要 Remix 一个升级版，请选择 **🪄 Make Variations**。启用 Remix 时，变体按钮变为绿色而不是蓝色。您可以在使用 Remix 时切换模型版本。



当您完成 `Remix` 后，请使用 `/settings` 或 `/prefer remix` 命令将其关闭。
在弹出窗口的提示中没有修改选项时，会创建标准变体。



| **步骤1**line-art stack of pumpkins艺术线条南瓜![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/d203f2e0ba7075c1713447424.png_q900)启用 Remix 模式，并选择一个图像网格或放大的图像进行 Remix。 | **步骤2** Remix 设置混合![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/16431355bceae571713447427.png_q900)选择“制作变化”。在弹出的窗口中修改或输入新提示。 | **结果** pile of cartoon owls 一堆卡通猫头鹰![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/938a10b216791381713447429.png_q900)Midjourney Bot根据原始图像的影响生成新的图像。初始图像是Midjourney生成的南瓜堆的线图。 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 开始图像![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/9a0080387f5ae661713447433.png_q900)**line-art stack of pumpkins** | 更改模型![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/5513b2a1df2d45f1713447436.png_q900)**line-art stack of pumpkins** **--test** | 更改主题![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/5cc0af93252431713447439.png_q900)balloon-animal shaped stack of pumpkins" |
| 介质变更![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/05647edfc705c871713447444.png_q900)vibrant illustrated stack of fruit |                                                              |                                                              |

### 使用混合参数

在使用混合处理时，您可以增加或删除参数，但必须使用有效的参数组合。改变 `/imagine prompt illustrated stack of pumpkins --version 3 --stylize 10000 to illustrated stack of pumpkins --version 4 --stylize 10000` 会返回错误，因为 Midjourney 模型版本 4 与样式参数不兼容(0-1000)。

使用混合处理只能使用有效参数：

|                       | **影响初始生成** | **影响变异** |
| --------------------- | ---------------- | ------------ |
| Aspect Ratio* 纵横比  | ✓                | ✓            |
| Chaos 混沌            | ✓                |              |
| Image Weight 图片权重 | ✓                |              |
| No 否定移除           | ✓                | ✓            |
| Quality 品质          | ✓                |              |
| Seed 种子             | ✓                |              |
| Same Seed 相同的种子  | ✓                |              |
| Stop 停止             | ✓                | ✓            |
| Stylize 样式化        | ✓                |              |
| Tile 平铺（四方连续） | ✓                | ✓            |
| Video 视频            | ✓                | ✓            |

- 改变宽高比将会拉伸图像，但不会扩展画布、添加缺失的细节或修复糟糕的裁剪。

## 如何激活 Remix

### 利用设置命令

输入 `/settings`，并从弹出菜单中选择`Remix`。🎛️ Remix

### 利用 Prefer Remix 命令

输入 `/prefer remix` 来切换 Remix模式的开启与关闭。

![image.png](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a7380f87165674c1713447415.png_q900)