#  MJ双冒号权重的分配和影响范围详解
---
## 什么是权重，多重提示？该如何使用它

我们可以通过向每个 Prompt 添加权重值 (例如 ::2)来控制混合效果的工作方式。 数值越低的 Prompt 对最终输出效果的影响就越小；数字越高的 Prompt 对最终输出效果的影响就越大。



您可以使用这些权重值来影响它在混合最终图像中的作用：

（末尾的数字对前面文字prompt的影响）

```plain
Prompt  最终的效果中具有较大强度影响 ::1.5
Prompt  默认强度 ::1
Prompt  最终效果半强度影响 ::0.5
Prompt  最终的效果中被减弱或删除 ::-0.5
```



权重符号 :: 影响的范围是从前一个 :: 到下一个 :: ，即被 :: 包围住的部分。如下所示，️️请注意如果 :: 符号后面没有数字，则其值默认为1.



译者注：下面是一个完整的 Prompt 示例，不是多个示例忘记换行

此处的关键词权重为二:: 2 , 此处的关键词权重为三::3 , 此处的关键词权重为负一::-1 , 此处的关键词权重为一:: , 此处的关键词权重为二:: 2



此提示的总权重为2+3-1+1+2=7

如果提示的总权重非常接近0（例如0.1)，最终混合的效果可能会变的... 奇怪。

提示词权重值之间的关系可以大致理解为，加权平均值的规则。 加权平均值是一种将不同的 values（在我们的例子中是 Prompt）组合以获得总平均值（在我们的例子中是最终混合图像）的方法，但每个 values（即 Prompt)被赋予了不同的权重（::n）或重要性。 这意味着 “Promptlet::5、Promptlet::10 ”与 “Promptlet::1、Promptlet::2” 的效果是一样的。

译者注：这一段的意思就是，一段咒语里的权重 ::n, 是按比例分配的，即 ::5, ::10 是两倍关系，所以它和 ::1, ::2的效果是一样的。



\----------------------------------------------

**The Slider Method**

您可能会发现重复部分 Prompt 对创造您想要的效果很有帮助，就像这样，

A fat black cat sleeps on the window sill:: fat::0.5

这实际上在“fat”这个词上放置了一个“控制值”，允许您增加/减少猫的肥胖度。

| 加权重 ::0.5                                                 | 加权重 ::0.1                                                 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| A fat black cat sleeps on the window sill:: fat::0.5         | A fat black cat sleeps on the window sill:: fat::0.1         |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/7f2cbb204d27cbf1713433948.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/a32867b0743660d1713433948.png_q900) |
| 权重0.5的猫更胖一些                                          |                                                              |



官方补充说明

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/b0970e6165a76011713433947.png_q900)



**The Scene Method**

您可能会发现使用第一组 Prompt 来设置场景，第二组 Prompt 填充场景很有帮助，就像这样

coffee house, twilight atmosphere:: two friends argue about money::

| 加了双冒号 ::                                                | 没加双冒号                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| coffee house, twilight atmosphere:: two friends argue about money:: | coffee house, twilight atmosphere, two friends argue about money |
| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/d3b033a492e4a0b1713433972.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/7c304be828621713433980.png_q900) |
| 左边场景部分要完整些，右边更侧重在人上                       |                                                              |



**The Puppeteering Method**

You can also use the blending effect of multi-prompts for puppeteering （这里链接了另一篇内容，以后空了翻）



## 我的多重提示 (multi-prompts)有什么问题？

当 weights/multipromt 似乎偏离所想时，通常是因为其中一个 Prompt 太不完整（几乎是语法上的？），以至于Midjourney 无法理解它。



有人会发出这样的提示：

female ninja, kneeling, infinity pool:: brilliant::1.5



这不起作用，因为 brilliant 没有主体，而且，作为一个单独考虑的 Prompt，Midjourney 需要更多关于在哪里应用它 (brilliant)的指示。



在这种情况下，我们可能会建议把所有的东西都放在一起，因为这是一个简单的句子：

female ninja kneeling in a brilliant neon infinity pool



如果艺术家发现 brilliant 是弱的，没有恰当的地表达出来，我们可能会建议在它上放上虚拟滑块 (译注：前面的The Slider Method)，这样你就可以调整它影响的强/弱。

female ninja kneeling in a brilliant neon infinity pool:: brilliant neon::0.5

请注意第二个 Prompt 是如何通过连接主体来连接第一个 Prompt 的。 并注意它是如何使用完全相同的关键词的。 这种方法似乎相当（但并非完全）可靠。



有些情况下，你不需要重复主语，你只需要重复单词或短语（精确到最后一个字母）。

a fat orange cat sleeps on a windowsill:: fat::0.2

给 fat 加上权重，让它变得更胖或不那么胖。



但是下面这个例子，权重也许**不会**生效，或者根本就不会有效

a fat orange cat sleeps on a windowsill:: chubby::0.2

\* chubby是fat的同义词  



我们看到的另一层关系是，背景与前景。

A twilight cafe:: Two friends talk about coffee

这很有效，因为 a twilight Cafe 作为一个独立的 Prompt 是有效的，关于 Two friends 的部分也是如此。

这是一个很好的方法来创建一个设定或场景，然后把主体放进去。