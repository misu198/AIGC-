# Midjourney 参数详解-Chaos 混沌

---

`--chaos`参数影响初始图像格多样性。高`--chaos`值将产生更不寻常和出乎意料的结果和构图。较低的"`--chaos`"值具有更可靠，重复的结果。



混沌接受 0-100 的值。

默认的混沌值为0。

### 混沌对工作的影响

#### 低混乱值

使用低混沌数值或者不指定数值将会在每次运行工作时产生略微变化的初始图像。

prompt 示例: imagine/ prompt watermelon owl hybrid

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/9fa15049ab1d5c21713438980.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6d2467129dc15951713439047.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/19db6ffc04e59e61713439042.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/2cb70f9cdd2baf61713439034.png_q900) |

#### 高混沌值

使用更高的混沌值将产生更多样化和意外的初始图像，每次运行任务时都会有所不同。

prompt 示例: imagine/ prompt watermelon owl hybrid --c 50

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/04d2d76fcc39e9f1713439024.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/abc420a3b6b4b071713438980.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/4b653bdbfd42b181713438982.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/e99889f79be8d671713439016.png_q900) |

#### 非常高 - 混沌值

使用极高的混沌值会产生多变的最初图像，每次运行任务时都有意想不到的组合或艺术形式。

prompt 示例: imagine/ prompt watermelon owl hybrid --c 100

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/f9bec7b95b8c7cb1713439009.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/423ddd3827796421713439002.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a4d7031f48875441713438994.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/666a79871df55ae1713438983.png_q900) |

### 如何更改混沌值

请使用`--chaos`或`--c`参数。

在您的提示符末尾添加“`--chaos <0-100数值>`”或“`--c <0-100数值>`”。

![MJ_Parameter_Chaos.gif](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/5e73dbd05737a321713438985.gif_q900)