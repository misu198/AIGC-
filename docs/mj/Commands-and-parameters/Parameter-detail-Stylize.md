# Midjourney 参数详解-Stylize 风格化

---

这个 Midjourney 机器人已经被训练出能够生成有艺术色彩、构图和形式感的图片。

`--stylize`或`--s`参数会影响应用该训练的强度。低`stylization`值会产生与 Prompts 相匹配但不太艺术化的图像。高`stylization`值则会创建非常艺术化但与 Prompts 联系较少的图像。

当使用默认 [V4模型] 时，`--stylize`的默认值为 100，并接受 `0-1000` 之间的整数值。

**不同版本 Midjourney 模型具有不同范围的样式化**。

|      |                | **Version 5** | **Version 4** | **Version 3** | **Test / Testp** | **niji** |
| ---- | -------------- | ------------- | ------------- | ------------- | ---------------- | -------- |
|      | Stylize 默认值 | 100           | 100           | 2500          | 2500             | NA       |
|      | Stylize 区间   | 0–1000        | 0–1000        | 625–60000     | 1250–5000        | NA       |

## 通用 Stylize 设置

### Midjourney V4 模型

prompt 示例: **/imagine prompt** **illustrated figs --s 100**

| **--stylize 50**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/1e2eff05f307dd1713438854.png_q900)**🖌️ Style Low** | **--stylize 100** (default)![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/0a12940e10bd91713438861.png_q900)**🖌️ Style Med** |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **--stylize 250**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/cb9b6f87ff305261713438868.png_q900)**🖌️ Style High** | **--stylize 750**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/72b4d4edbcd013e1713438834.png_q900)**🖌️ Style Very High** |

### Midjourney V5 模型

prompt 示例: **/imagine prompt** **colorful risograph of a fig --s 200**

| **--stylize 0**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/6bedf63eb97991e1713438878.png_q900) | **--stylize 200** (default)![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/1ab750de336fb8a1713438835.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **--stylize 400**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/03dd26fe7ba694c1713438888.png_q900) | **--stylize 1000**![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/62328fc055d68551713438837.png_q900) |

## 如何切换`stylize`值

#### 使用 `--styleze` 参数

在 prompts 末尾添加 `--styleze <styleze 值>` 或 `--s <styleze 值>` （不同版本范围不一样）

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/1d673f4babeedab1713438837.gif_q900)

#### 使用设置命令

输入`/settings`并从菜单中选择您喜欢的`stylize`值即可。

**🖌️ Style Low**  **🖌️ Style Med** **🖌️ Style High** **🖌️ Style Very High** 