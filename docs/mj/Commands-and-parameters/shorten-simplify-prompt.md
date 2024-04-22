# shorten 分析简化 prompt

---

这个命令可以让你“**分析**”一个提示，获取可能无效的词汇建议以及可能关键的词汇。



使用一个群友的 prompt 测试:

```plain
extreme-close,3D llustration, Vibrant Girl, bright makeup ideas::2, Dreamcore, Highlighting, delicate skin, edge light, 3D, blender, oc rendering, ray tracing, extreme details, super realistic, CGI
```



## 输入命令： /shorten prompt

```
**/shorten** extreme-close,3D llustration, Vibrant Girl, bright makeup ideas::2, Dreamcore, Highlighting, delicate skin, edge light, 3D, blender, oc rendering, ray tracing, extreme details, super realistic, CGI
```

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/763ac2ce5894ad51713438539.png_q900)



### 看看中文翻译更直接一点：

#### 重要的标记 (帮你标记了生效的：重要和一般的，并用删除线标记出无效的词)

```
**极近距离，3D**插图，**活泼的女孩，明亮的化妆思路::2**，梦幻风，高光，**娇嫩的皮肤**，边缘光，3D，混合器，oc渲染，光线追踪，极致细节，超现实，CGI，
```

#### 缩短的提示

1️⃣ 极近距离，3D插图，活泼的女孩，明亮的化妆思路::2，梦幻风，高光，娇嫩的皮肤，CGI

2️⃣ 极近距离，3D插图，活泼的女孩，明亮的化妆思路::2，娇嫩的皮肤

3️⃣ 极近距离，3D，活泼的女孩，明亮的化妆思路::2，娇嫩

4️⃣ 极近距离，3D，活泼的女孩，化妆

5️⃣ 近距离，3D，活泼，化妆

点击一个按钮来实现其中一种缩短的提示。



### Show Details 查看细节

点击 “Show Details” 可以查看分析细节

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/2c666c7e025bf4f1713438540.png_q900)



**多出的更详细的分析细节，关键词的权重占比数字， 是不是很直观！**

**extreme**(0.55)-**close,3D**(0.82) llustration (0.09), **Vibrant**(1.00) **Girl**(0.53), **bright**(0.19) **makeup**(0.86) **ideas::2**(0.30), Dreamcore (0.08), Highlighting (0.07), **delicate**(0.19) skin (0.09), edge (0.01) light (0.03), 3D (0.01), blender (0.01), oc (0.00) rendering (0.01), ray (0.02) tracing (0.02), extreme (0.04) details (0.00), super (0.00) realistic (0.03), CGI (0.04),

------

**极**(0.55)-**近,3D**(0.82) llustration (0.09), **充满活力的**(1.00) **女孩**(0.53), **明亮**(0.19) **化妆**(0.86) **思路::2**(0.30), Dreamcore (0.08), Highlighting (0.07), **精致的**(0.19) skin (0.09), edge (0.01) light (0.03), 3D (0.01), blender (0.01), oc (0.00) rendering (0.01), ray (0.02) tracing (0.02), extreme (0.04) details (0.00), super (0.00) realistic (0.03), CGI (0.04),

------

██████████ Vibrant  充满活力的

█████████░ makeup 化妆

████████░░ close,3D 近 3D

█████░░░░░ extreme  极端，极限

█████░░░░░ Girl 女孩

███░░░░░░░ ideas::2 思路想法

██░░░░░░░░ bright 明亮的

██░░░░░░░░ delicate 精致的；易碎的；微妙的；敏感的



当然你可以直接点击对应的 `1` `2` `3` `4` `5` 直接应用(/imagine)调整后的 prompt 