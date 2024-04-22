# Midjourney 高级 Prompts-Zoom Out 视角扩大

---

“**Zoom Out**”实际上是将画面的内容进行了扩展,就像在一个窗口里缩小图片或者调整相机镜头的焦距，而并非在视觉上实现缩小，所以将其翻译为"缩小"的确可能会让人产生混淆。这里我翻译为"视角扩大"，这样更能准确地传达原文的意思。

【Midjouney zoom out 创建无限放大】 社群成员：**新裤头儿 创作**

视角扩大选项允许你扩大一个放大图像的画布超出其原始边界，而不改变原始图像的内容。新扩展的画布将根据提示和原始图像的指导填充。

画面外扩并不会增加图像的最大尺寸，仍然为 **1024px x 1024** px。

## 画面外扩

在视角扩大图像后，将出现 **🔎 Zoom Out 2X** **🔎 Zoom Out 1.5X** 的按钮。



提示词: `**vibrant California poppies**`

| 起始图像                                                     | 外扩1.5X                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/dd319f41326983b17134392531713439503.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/fdad33fce85f0ff17134392541713439510.png_q900) |
| 展示提示中活泼的加利福尼亚罂粟的示例图像                     | 示例图像以提示活泼的加利福尼亚罂粟为基础，扩展到外扩50%      |
|                                                              |                                                              |











外扩2X![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/8c700488f7846e31713439275.png_q900)

示例图像以提示活泼的加利福尼亚罂粟为基础，扩展到外扩100%





## 调整为正方形

使用 **Make Square**，你可以调整一个非正方形图像的宽高比，使其变成正方形。如果原始宽高比是宽（横向），它将在垂直方向扩展。如果是高（纵向），它将在水平方向扩展。标记 `↔️` `↕️` 在 **↔️ Make Square** 按钮旁边，也指示了图像将被哪个方向扩展。 **↔️ Make Square** 按钮将出现在非正方形放大图像下方。



提示词: `**vibrant California poppies**`



| 起始图像 示例图像的提示为活泼的加利福尼亚罂粟                | **↔️ Make Square** 示例图像的提示为活泼的加利福尼亚罂粟，外扩画面以填充宽高比为正方形 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/adde335cbcf64c317134392811713439606.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6085bb4b7b52a2517134392531713439626.png_q900) |
| 起始图像 示例图像的提示为活泼的加利福尼亚罂粟                | **↔️ Make Square** 示例图像的提示为活泼的加利福尼亚罂粟，外扩画面以填充宽高比为正方形 |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/54fef27dd915ce317134392921713439717.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/3f4457d16a8417134392561713439726.png_q900) |











## 

## 自定义视角扩大

**🔎 Custom Zoom**  按钮让你选择图像外扩的多少。在放大图像下的 **🔎 Custom Zoom** 按钮会弹出一个对话框，你可以输入一个自定义的 `--zoom` 值。 `--zoom` 接受 **1-2** 之间的值。



**更改放大图像的宽高比**

你可以在这个自定义外扩弹出框中使用 `**--zoom 1**` 来更改宽高比，使用 `**--ar**` 参数，不进行外扩。



### 改变你的提示与自定义外扩

**🔎 Custom Zoom** 允许你在扩展图像前更改提示，让你对完成的图像有更精细的控制。例如，将提示改为"**A framed picture on the wall**"，得到这样的结果：





| 起始图像                                                     | 自定义外扩 + 改变的提示                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **prompt: vibrant California poppies**                       | 外扩提示：**A framed picture on the wall** --zoom 2          |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/9a40870d83258fe17134392991713439823.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/068bda3fccd822417134392561713439840.png_q900) |











## 其它玩法

老外已经开始用套娃玩视频了，耐心的（zoom 降低，多出图（关键帧））会做的比较丝滑，群主比较没耐心（zoom 2x） 试了个怪怪的登西……

**MJ zoom out + runway** **帧插值**