# 如何教ChatGPT写AIGC 绘图关键词 Prompt
---
想用Midjourney 生成漂亮的AIGC图片，但词穷+缺少专业知识，无法舌灿莲花的把想法传递给Midjourney。这个时候，可以充分发挥文学大师ChatGPT的所长，利用GPT来完善idea的细节文字。



众所周知，ChatGPT的数据库里不包含Midjourney prompt相关的知识，但是我们可以教它，把ChatGPT变成一个私人prompt助理。



## 先说两个极简单但付费的方法：

1. 在discord频道引入一个ChatGPT bot，然后直接让它生成prmopt就可以了
   优点：使用方便，在个人频道里直接调用即可
   缺点：没有官方的bot，第三方的bot 服务不稳定，且免费次数用完后会收费 ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a7c1043f6d5a3f61713434489.png_q900)
2. 付费成为ChatGPT 4.0的用户，4.0 可以读图，能列出图片特征。（试过New bing，被阉割了）



下面开始正文



## 普通穷人的方法，教ChatGPT3.5 如何生成prompt

大体思路是：

1. 告诉chatGPT 根据我们的idea，生成舌灿莲花般的文字
2. 让chatGPT根据prompt 公式，把文字整理成midjourney 使用的格式
3. 教完以后，在这个Chat内，以后发idea 给它就可以直接生成prompt了

### 初级版 （强随机性，适合脑爆）

请根据我给你的idea，详细描述一个富有创意的画面。 然后使用逗号分隔描述里的修饰词并把描述翻译成英文。

idea: 一只鸟

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/7ea703273d1daf11713434466.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/35d4f1f9d4a08591713434466.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

也可以要求ChatGPT 一次出5个画面描述。（一次出太多GPT容易崩在网络故障上）

### 中级版（教公式）

告诉GPT，prompt一些常见的公式
例如：[主体，主体描述] + [细节, 修饰词, 氛围] + [艺术风格, 质感, 视角, 渲染器] + [MJ 参数]

根据主体和自己的习惯定义这个公式，并告诉ChatGPT

Tips：分步教，一次教太多，它会漏掉一部分内容

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/ced38442fce97441713434465.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a4cbda08bbd3a0c1713434465.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

### 中级Plus 版

告诉ChatGPT，一些常用的关键词和MJ 参数

例如添加照片质感的关键词和参数 “以后prompt 里要求照片质感时，请在描述末尾添加 “photography, reality, 4k, high detail --v 5”，理解的话，请回答明白”

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/c96f586b9a7e8791713434465.png_q900) | ![img](https://image.bzu.cn/web_img/202307/6b1519c7cdfa884.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |