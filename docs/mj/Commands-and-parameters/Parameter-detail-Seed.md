# Midjourney 参数详解-Seed 种子

---

Midjourney 机器人使用一个种子号码创建了一个视觉噪声场，类似于电视静态图像，作为初始图像的起点生成。每个图像的种子号码都是随机生成的，但可以通过`--seed`或`--sameseed`参数指定。使用相同的种子号码和提示将产生类似的结果图像。



`--seed` 接受 **0 - 4294967295** 之间的整数。

`--seed`值仅影响初始图像网格(指4张图形成的网格)。

种子值模型版本`1`、`2`、`3`、`**test**` 和 `**testp**` 是非确定性的，并且会产生相似但不完全相同的图像。

使用相同的`提示+种子+参数`在模型版本`4`、`5`和`niji`中将产生相同的图像。

## 种子参数

如果未指定种子，则 Midjourney 将使用随机生成的种子编号，每次使用提示时产生各种各样的选项。

#### 运行三次（使用随机种子）：

prompt 示例: /imagine prompt celadon owl pitcher

![image.png](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/4f1a2ec4ef283af1713438928.png_q900)

#### 运行两次使用 `--seed 123`：

prompt 示例: /imagine prompt celadon owl pitcher --seed 123

| ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/c254a39d21a73131713438936.png_q900) | ![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/c6a3e381ae267da1713438913.png_q900) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

### 同种子参数

“`--seed`值会创建一个单一的大随机噪声场，应用于初始的图像网格中的所有图像。当指定`--sameseed`时，初始网格中的所有图像都使用相同的起始噪声，并且会生成非常相似的图像。”

`--sameseed`接受 **0 - 4294967295** 的整数。

`--sameseed`只兼容 1、2、3 版本，test 和 testp 版本。

| 早期的视觉噪音--sameseed![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/4d8ce38634c7ce61713438912.png_q900)--sameseed 12345 | 工作完成--sameseed![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/3855548b8bf5b11713438945.png_q900)--sameseed 12345 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 早期的视觉噪音(无)--sameseed![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/470af5cd9eb631713438952.png_q900)--sameseed 12345 | 工作完成(无)--sameseed![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/f524fa3593b769a1713438914.png_q900)--sameseed 12345 |

## 如何查找工作的种子编号

#### 使用 Discord  ✉️  表情符号

通过对工作进行 ✉️ 信封表情符号来在 Discord 中查找工作的种子编号。

![MJ_JobID_EmojiReact.gif](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/3e3662ce8df4f691713438916.gif_q900)

#### 使用 show 命令显示以前的生成任务

要获取过去图像的种子号码，请复制 Job ID，并使用该 ID 的 `**/show <Job ID #>**` 命令来恢复工作。然后，您可以使用 ✉️ 信封表情符号对新生成的作业进行交互触发（再发给你自己存起来）。

## 如何应用种子编号

### 使用 `--seed` 或 `--sameseed` 命令

在 prompts 末尾添加 `--seed <0-4294967295间的一个值>` 或 `--sameseed <0-4294967295间的一个值>`

![MJ_Seed_Gif.gif](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/e93968c139d0d01713438963.gif_q900)