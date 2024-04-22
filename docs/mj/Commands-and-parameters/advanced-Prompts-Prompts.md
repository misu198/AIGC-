# Midjourney 高级 Prompts-多重 Prompts

---

Midjourney Bot 可以考虑两个或更多个单独的概念，使用`::`作为分隔。分隔 prompt 允许您对 prompt 的不同部分分配相对权重。

## 多 Prompt 基础知识

在 Prompt 中添加双冒号`::`表示 Midjourney Bot 应该单独考虑每个部分。

在下面的例子中，针对 Prompt 的"**热狗**"，所有单词都被视为一个整体，Midjourney机器人会生成美味热狗的图片。如果将提示分成两部分，"**热**"和"**狗**"这两个概念会被单独考虑，从而创造出一张热的狗的图片。

双冒号`::`之间没有空格。

多提示工作于模型版本1、2、3、4和 niji。

任何参数仍然是添加到 Prompt 的最后。

| hot dog![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6247574a6c7a1661713438407.png_q900)热狗被认为是一个单一的概念。 | hot:: dog![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/b741470545d825d1713438399.png_q900)"热和狗" 被认为是两个不同的想法。 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| cup cake illustration![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/ffab0da7dddf9eb1713438272.png_q900)杯子蛋糕插图被认为是一起制作杯子蛋糕的图像。 | cup:: cake illustration![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/c094e34acc445ae1713438386.png_q900)将杯子与蛋糕图示分开考虑，制作杯装蛋糕的图片。 |
| cup:: cake:: illustration![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/0601f43fc958f7a1713438272.png_q900)杯子，蛋糕和插图被单独考虑，产生了一个杯子蛋糕，并带有常见的插图元素，如花朵和蝴蝶。 |                                                              |

## 提示权重

使用双冒号`::`将提示分成不同的部分时，您可以在双冒号后面紧跟数字（无空格）以指定该提示部分的相对重要性。

在下面的例子中，提示的“`hot::dog`”产生了一个热狗的图像。将提示更改为“`hot::2 dog`”使单词“**hot**”变得比“**dog**”重要两倍，从而产生一个非常热的狗的图像！



[模型版本] 1、2、3仅接受整数作为权重。

[模型版本] 4 可接受权重的小数位数。

未指定权重默认为 1。

| hot:: dog![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6b879973ee8bbfe1713438375.png_q900)热和狗被视为不同的思维。 | hot::2 dog![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/d12e14728002b121713438274.png_q900)"`热`的重要性是`狗`的两倍" |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

### 权重已归一化

- `hot:: dog` 与 `hot::1 dog`，`hot:: dog::1`，`hot::2 dog::2`，`hot::100 dog::100`等相同。
- `cup::2 cake` 和 `cup::4 cake::2`, `cup::100 cake::50` 等相同。
- `cup:: cake:: illustration` 和 `cup::1 cake::1 illustration::1`, `cup::1 cake:: illustration::`, `cup::2 cake::2 illustration::2` 等相同。

### 负面提示权重

负权值可以添加到 Prompts 中，以消除不需要的元素。所有权重的总和必须是正数。

| vibrant tulip fields![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/54a4c65095cda911713438364.png_q900)充满活力的郁金香田 | vibrant tulip fields:: red::-.5![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/ee5cb9f86a779c41713438370.png_q900)充满活力的郁金香田：红色： -0.5 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

郁金香田里很少有红色的花。

**权重已被规范化，因此：**
`tulips:: red::-.5` 和 `tulips::2 red::-1`, `tulips::200 red::-100`, 等相同。

### --no 参数

“`--no`”参数相当于将多个 prompt 中的一部分权重设置为“`-.5`”鲜艳的郁金香田野`::red::-.5`相当于鲜艳的郁金香田野`--no red`。