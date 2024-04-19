# 👋 欢迎

import DocsCards from '@site/src/components/DocsCards'
import DocsCard from '@site/src/components/DocsCard'
import polestarbanner from './assets/img/PoleStar_banner.png'

## 关于本教程

本教程包含两个部分，内容是我在学习 Prompt Engineering 过程中，总结出来的一些经验和方法。如果你也在学习，希望这份教程能够帮到你。

<DocsCards>
  <DocsCard
    header="深入浅出人工智能"
    href="docs/ai-101"
    icon="/static/icons/polestarlogo.png"
  >
    <p>一份人人都能看懂的人工智能教程。目前正在全力撰写中。敬请期待。</p>
  </DocsCard>
  <DocsCard
    header="ChatGPT 教程"
    href="docs/chatgpt-learning-path"
    icon="/static/icons/openai-fill.png"
  >
    <p>
      由浅入深，从使用者的角度，教你如何使用 ChatGPT，以及如何更好地使用
      ChatGPT。
    </p>
  </DocsCard>
  <DocsCard
    header="Midjourney 教程"
    href="docs/midjourney-learning-path"
    icon="/static/icons/midjourneylogo.png"
  >
    <p>
      通过各种场景案例，教你如何使用
      Midjourney。即使是小白，看完教程后，也能够快速上手。
    </p>
  </DocsCard>
</DocsCards>

<br />

它不是什么？

- 本教程不是 prompt 大全，如果你预期是找到能直接用的 prompt，建议你谷歌找一找。本教程更多地是教你方法，以及解释这些方法为何有效。
- 本教程不是权威指南，在这个领域我也只是学生。

## 如何阅读？

很感谢你打开这份教程，但我建议你在阅读这份教程的时候：

1. **降低预期：** 我不是专家，我也在学习，我只是比你多走了几步而已。教程里的内容难免会有遗漏或错误。另外，我这份教程，目标读者是初学者，所以在教程中，为了让大家更容易理解，难免会用到不太准确的类比，或者用词，请各位见谅。
2. **不要吝啬你的反馈：** 如果你遇到无法看懂的地方，亦或者我写错了的地方，不妨给我提个 Issue 或者填写这个表单。我们共同进步，并为 PE 的科普出一份力。
3. **通过输出倒逼输入：** 最好的学习方法就是实操，教程里会提供不少案例，你边阅读，边尝试。甚至如果可以的话，不妨将你写的 prompt 通过 Issue 或表单的方式，分享给我，我会将不错的案例加到文档内。

另外，我一直认为最好的学习方法，就是实践，所以我建议你使用 ChatGPT 或者 Midjourney 上 运行一下教程里的案例。这样能够记得更牢靠一些。

最后，在读文档的过程中，你会看到以下几个 emoji：

- 🚧 ：标有这个 emoji 代表内容，我还需要进一步去完善补充，但并不影响你的阅读。我会在后续迭代补充。
- 🆘 ：这个代表我需要各位的帮助，比如有可能是希望大家给我一些某场景的 prompt 案例等。如果你有想法，不妨通过 Issue 或，向我反馈。
- 🔴：为了让大家能更平滑地学习高级篇的内容，我会在基础篇提一些高级篇的概念，当你看到这个红色圆时，就表示这是高级内容，你可以不深究，先了解即可。

## 如何贡献一份你的力量？

如果可以的话，不妨在 [Github Page](https://github.com/thinkingjimmy/Learning-Prompt) 上给我点赞，或者将本教程分享给其他人。感谢~

在阅读这个文档的时候：

1. 遇到错别字、句子不通顺，亦或者读不懂的地方，欢迎通过 Issue 或通过我们的 [Discord 频道](https://discord.gg/B7Z7wjuUPg)反馈给我，我会对其进行修改。一经采纳会将你的名字罗列在感谢人名单内。
2. AI 的发展非常快，今天写的教程，很有可能明天就过期了。如果你在文档里看到有什么落后的内容，比如某些指令已经不需要了，或指令不生效了，也欢迎通过 Issue 或通过我们的 [Discord 频道](https://discord.gg/B7Z7wjuUPg)向我反馈。
3. 看到标有 🆘 的内容，然后你又有不错的想法，不妨通过 Issue 或通过我们的 [Discord 频道](https://discord.gg/B7Z7wjuUPg)向我反馈你的想法。

在感谢人名单页面里，我会罗列帮助过我的朋友们 😁

## 不妨看看我的其他产品？

除了此教程外，我还制作了其他付费内容产品，感兴趣的朋友可以看看：

- [播客小捕手：](https://xiaobot.net/p/xiaobushous1?refer=599951e8-47eb-4898-aa3b-a7d0a1a06b0f)如果你喜欢播客，不妨看看，未来我会在上面尝试更多 AI 相关的想法。
- [随意搜寻 | 2023](https://xiaobot.net/p/suiyisouxun2023?refer=599951e8-47eb-4898-aa3b-a7d0a1a06b0f) ：我的付费 newsletter，每周更新。

另外，我和我的朋友一起开发了一款 AI 应用。如果因为一些网络原因，你无法使用 ChatGPT，你可以试试我们开发的产品 [PoleStar Chat](https://github.com/thinkingjimmy/PoleStarChat):

<img src={polestarbanner} width="1024" />

## 特别鸣谢

本教程制作过程中，内容和案例参考了以下教程或文档：

ChatGPT:

1. [Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)
2. [Learn Prompting](https://learnprompting.org/)
3. [ChatGPT3-Free-Prompt-List](https://github.com/mattnigh/ChatGPT3-Free-Prompt-List)
4. [Natural Language Processing with Deep Learning](http://web.stanford.edu/class/cs224n/slides/cs224n-2023-lecture11-prompting-rlhf.pdf)
5. [edx ChatGPT101](https://www.edx.org/course/introduction-to-chatgpt)
6. [OpenAI Examples](https://platform.openai.com/examples)

Midjourney:

1. [Midjourney Guide](https://docs.midjourney.com)
2. [Midlibrary](https://www.midlibrary.io/)
3. [Aituts](https://aituts.com/)
