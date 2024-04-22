# 如何在MJ里使用负向提示词（示例）
---
您可以使用负面提示来指定您在Midjourney生成中不想要的内容。以下是一个使用负面提示的示例：

当您在提示中使用“绘画”一词时，您将获得挂在墙上的绘画照片，有时还带有框架和家具。假设您只想要绘画本身。您将使用负面提示来摆脱所有额外的细节：

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/95aead4fbfb4cee1713434367.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6afcd1f69f3b0be1713434386.png_q900) |
| modern abstract painting --seed 1                            | modern abstract painting --seed 1 **--no frame furniture wall** |

提示：将所有负向提示都放在--no之后，没有必要为每个单独的事物都写一个 --no

## 有效的负面提示示例

### 使用负向提示来摆脱手

Midjourney不能很好地处理手（尚未）。如果您得到了太多奇怪的手，为什么不隐藏它们呢？”

（译者注：现在v5 已经改善了对手的处理，这里更多是从例子里感受到负向提示的用法）

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/53bdbfc5e9d98a71713434367.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/8c426be8f5176dd1713434367.png_q900) |
| blonde girl leaning on table and smiling at camera, detailed facial features, detailed eyes, polaroid, 1990 | blonde girl leaning on table and smiling at camera, detailed facial features, detailed eyes, polaroid, 1990 **--no hands** |

### 使用负向提示词去除文字

文本是Midjourney不擅长的另一件事。您可以使用负面提示来摆脱文本。

（译者注：MJ已经发布关于改善文字的计划）



负向词越明确，效果越好。我使用了“--no text font letters”，这比仅使用“-no text”要好得多

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/8eb11348e3b01713434368.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/68b6025c9e5d0f31713434371.png_q900) |
| chicken logo, style of Milton Glaser                         | chicken logo, style of Milton Glaser **--no text font letters** |

您可以在此示例中看到，负向提示不仅消除了文本，而且还使图像更接近我想要的风格（纽约地铁地图设计师Milton Glaser）。当Midjourney不必专注于组合带有文本的标志时，它能够更好地模拟风格。



您可以在此处观察到类似的效果：

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/e327c9c068270a21713434370.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a04b1c12ff0fd31713434409.png_q900) |
| chicken logo, style of Egon Schiele                          | chicken logo, style of Egon Schiele **--no text font letters** |

当负面提示不包含文本时，最终结果更接近艺术家的实际风格。

这是一个转化的好方法：

### 使用负面提示来获得您想要的风格

这是我尝试的提示。虽然原始结果很漂亮，但它们根本**不是**我想要的。

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/11917bbf8e3ba5a1713434370.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/49d19881937bc691713434371.png_q900) |
| anime stormtrooper by studio ghibli                          | anime stormtrooper by studio ghibli **--no 3d render realistic** |

我的假设是训练数据中有太多的3D和逼真的突击队战士。它完全压倒了提示的其余部分！

通过指定我在负面提示中不想要3D，我能够获得更接近我想要的结果。



### 在保持相同seed的情况下添加负提示

假设您已经有了一张喜欢的图片。 您想向其添加负提示。 但是，您不想 re-roll (新生成一组图），因为那会创建不同的图像。



只要您知道 Seed，就可以使用负提示重新创建相同的图像。

每个图像都有一个 Seed，具有相同seed的图像彼此相似。

找到 Seed后，您可以做很酷的事情，例如这样

| **Original**                                                 | **w/ Negative Prompts**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/cf464f3a6d48be81713434425.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/c73ab1801d4ffc31713434372.png_q900) |
| light watercolor, interior of a cozy cafe, bright, white background, few details, dreamy, Studio Ghibli --seed 3817455947 | light watercolor, interior of a cozy cafe, bright, white background, few details, dreamy, Studio Ghibli --seed 3817455947 **--no people person** |

## 备选方法：使用负图像权重

除了使用负提示之外，您还可以使用负权重来指定您在生成中不想要的内容。

有关权重的更多信息：

权重用于强调和减弱提示的不同部分。具有正权重的单词会被强调，而具有负权重的单词会被减弱。

我更喜欢使用权重而不是“-no”命令，因为它们可以精细控制提示的每个部分。以下是我如何使用权重编写上面的示例：

a**nime by studio ghibli::1.4 stormtrooper::1.2 3d render realistic::-1.5**

在提示的每个部分后面跟随 ::数字。

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/153abc6149af0021713434436.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/7205efc964f9b111713434372.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| anime by studio ghibli::1.4 stormtrooper::1.2 3d render realistic::-1.5 | anime by studio ghibli::1.5 stormtrooper::1 3d render realistic::-1.5 |



-END-