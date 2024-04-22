# Midjourney 参数详解-Version 版本

---

Midjourney 定期发布新的模型版本以提高效率、连贯性和质量。最新的模型是默认的，但可以使用`--version`或`--v`参数或使用`/settings`命令并选择一个模型版本来使用其他模型。不同的模型擅长处理不同类型的图像。



`--version`接受值1、2、3、4和5。

`--version`可以缩写为`--v`。

## 最新模型

Midjourney V5 模型是最新且最先进的模型，于2023年3月15日发布。要使用此模型，请在提示后添加 `--v 5` 参数，或者使用 `/settings` 命令并选择 `5️⃣ MJ Version 5`。



该模型具有非常高的连贯性，在解释自然语言提示方面表现出色，分辨率更高，并支持诸如 `--tile` 等高级功能。 

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/ade0fae7eb61ba61713438756.png_q900)***Prompt: vibrant California poppies --v 5\*** | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/70d9d2354bc9d4f1713438761.png_q900)***Prompt: high contrast surreal collage --v 5\*** |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

## 当前模型

Midjourney V4 模型是全新代码库和全新 AI 架构设计而成，并在 Midjourney AI 超级集群上进行训练。最新 Midjourney 模式具有更多关于生物、地点、对象等知识。它能够更好地捕捉小细节，并能够处理包含多个角色或对象等复杂提示。Version 4 模式支持像图像 prompts 和多重 prompts 这样的高级功能。

**该模型具有非常高的连贯性，在图像 prompts 方面表现出色。**

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/510e9e4d14d7fd61713438744.png_q900)***Prompt: vibrant California poppies\*** | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/867a089c31abc321713438745.png_q900)***Prompt: high contrast surreal collage\*** |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

## 版本 4 的 4a，4b 和 4c

Midjourney 模型版本 4 有三种略微不同的“风味”，对模型的风格调整进行了轻微调整。通过在 V4 提示的末尾添加`--style 4a`、`--style 4b`或`--style 4c`来尝试这些版本。

`--v 4 --style 4c` 是当前默认设置，无需在提示符的末尾添加。



4a 和 4b 风格的注意事项

--样式 4a 和 4b 仅支持`1：1`，`2：3`和`3：2`比例。

--样式 4c 支持宽高比达到 `1:2` 或 `2:1`。

## 以前的模型版本

你可以通过使用`--version`或`--v`参数或使用`/settings`命令，并选择一个模型版本来访问较早的模型。不同模型擅长处理不同类型的图像。

**prompt 示例:** **/imagine prompt vibrant California poppies --v 1**

| --version 3![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/cb6aca7176e628e1713438744.png_q900)default model: 07/22–11/22高度创意的作品 适度的连贯性 | --version 2![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6c94e06a19643fa1713438772.png_q900)default model: 04/22–07/22创意、色彩丰富、具有绘画感 低相干性 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| --version 1![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/1ef908fa174084d1713438746.png_q900)default model: 02/22–04/22非常抽象和具有画家特色 低相干性 | --hd (high definition)![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/0e3ebfb566924a01713438746.png_q900)早期替代型模型 繁忙的、详细的、抽象的 低相干性 |

## Niji 模型版本

Niji 模型是 Midjourney 和 Spellbrush 合作打造的，旨在产生动漫和插画风格。Niji 模型具备更多的动漫知识、动漫风格和动漫美学。它在动态和动作镜头以及人物成像方面表现出色。

**prompt 示例:** **/imagine prompt vibrant California poppies --niji**

| --v 4![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/70932a2662fe06c1713438747.png_q900)vibrant California poppies | --niji![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/39a62f606ec812b1713438786.png_q900)vibrant California poppies --niji |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| --v 4![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/01bda4a2132030a1713438747.png_q900)fancy peacock | --niji![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/380d76e473ddf741713438796.png_q900)fancy peacock --niji |

**关于**`**--niji**`**模型的笔记**

Niji 不支持`--stylize`参数。请使用`/settings`命令并选择`Style Med`来重置所有`--niji`提示的默认样式设置。Niji 支持多 prompts 或图像 prompts。



## 测试模型版本

偶尔会发布新模型供社区测试和反馈。目前有两个可用的测试模型：`--test`和`--testp`，可以与`--creative`参数结合使用，以获得更多样化的组合。

**prompt 例子:** **/imagine prompt vibrant California poppies --testp --creative**

| **--test**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/8a72b04ef60dc691713438803.png_q900)**A general-purpose artistic model with good coherency** | **--test + --creative**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/ec8e0506354bc51713438749.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **--testp**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/be595bcfedac8031713438749.png_q900)**A photo-realism model with good coherency** | **--testp + --creative**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6879dd9c13087841713438813.png_q900) |

测试模型仅支持“`stylize`”值在`1250`到`5000`之间。

测试模型不支持多 prompts 或图片 prompts。

测试模型的最大长宽比为`3:2`或`2:3`。

当纵横比为`1:1`时，测试模型仅生成**两个**初始网格图像。

仅当纵横比不为`1：1`时，测试模型只会生成**一个**初始网格图像。

prompt 前面的单词可能比后面的单词**更重要**。

## 如何切换版本

### 方法一、使用版本或测试参数（单次）

在 Prompts 末尾添加 `**--v 1**,` `**--v 2**`, `**--v 3**`, `**--v 4**`, `**--v 4**` `**--style 4a**`, `**--v 4**` `**--style 4b**` `**--test**`, `**--testp**`, `**--test**` `**--creative**`, `**--testp**` `**--creative**` 和 `**--niji**` 等参数



![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/39143d066a0188f1713438750.gif_q900)



### 方法二、使用设置命令（预设）

输入 `**/settings**` 在菜单选择你喜欢的版本，可根据需求进行设定，需要注意的是，在末尾添加其他模型指令将覆盖 `**/settings**` 设定的内容

**1️⃣ MJ Version 1** **2️⃣ MJ Version 2** **3️⃣ MJ Version 3** **4️⃣ MJ Version 4** **🌈 Niji Mode** **🤖MJ Test** **📷 MJ Test Photo**