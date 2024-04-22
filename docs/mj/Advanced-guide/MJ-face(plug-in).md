# MJ如何精准换脸（插件）
---
Github主页：[点击跳转](https://github.com/deepinsight/insightface/blob/master/web-demos/swapping_discord/README.md#disclaimer)

 😇 前言 

无意中看到了群友分享的Midjourney精准控脸插件，于是乎便搬运了过来，对于基于diffusion算法开发的midjourney，先天在内容的可控性上有一定的不足，所以该教程是采用的二次编辑的方法来实现人脸的精准控制，所以推荐在氛围、动作等等满意的情况下进行脸部替换。



本文99%为汉化GIT主页内容，老手可直接跳转[【此处】](https://tob-design.yuque.com/kxcufk/mj/xf15dghkqg1prygt#TVV6J)开始

 😃 正文 

对于超过 99% 的人来说，使用 Midjourney 创建自己的肖像是不可行的，除非你是一个在网上拥有数千或数百万张照片的名人。但现在，借助 InsightFaceSwap Discord 机器人，您只需几个步骤即可轻松完成此任务。

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd01713434231.jpg)



 📔 Discord 斜杠命令 

nsightFaceSwap 机器人可以通过以下命令帮助您：

 /保存IDname upload-ID-image 

用于上传注册自己的证件照或numpy特征，用于后续的换脸和修容。您最多可以永久上传 10 个实例并使用它们，而无需重复上传。

（正视、高画质、无眼镜、无厚刘海证件照优先。）

 /设置名称name(s) 

设置当前/默认身份名称，用于使用上下文菜单生成图像。如果需要设置多个ID名称，请使用逗号分隔。

 /列表编号 

列出所有注册的身份名称。

 /交付name 

删除特定身份名称。

 /删除 

删除所有注册名称。

 /敏捷name(s) upload-image 

用目标图像上的注册身份名称替换面部。

 👌 分步指南 

1请参考[此链接](https://docs.midjourney.com/docs/invite-the-bot)注册 Discord 应用程序，创建一个新的聊天室，并邀请 Midjourney 机器人加入聊天室。（老玩家可跳过）

2

通过以下链接邀请 InsightFaceSwap 机器人加入聊天室：

[点击跳转](https://discord.com/oauth2/authorize?client_id=1090660574196674713&permissions=274877945856&scope=bot)

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd11713434163.jpg)



3. 使用``/saveid`` 命令注册您的身份名称和特征。这里'mnls'是注册名称，可以是任意字母或数字，最多8个字符。如果一切顺利，机器人会告诉您保存成功。请注意，新创建的身份将自动设置为默认身份。



![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd21713434244.jpg)



4.接下来，我们可以尝试创建肖像。让我们开始吟唱 Midjourney 提示并放大其中一个输出。

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd31713434164.jpg)



5. 放大完成后，我们可以简单地使用``INSwapper``上下文菜单来生成我们的肖像。右键单击目标图像，然后选择“Apps-INSwapper”菜单。请注意，我们还可以使用 ``/setid`` 命令来更改默认身份名称。



![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd41713434164.jpg)



6. 一般任务不到一秒就完成，可以看到结果。



![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd51713434262.jpg)



7. 除了处理Midjourney 生成的照片，我们还可以显式地使用``/swapid`` 命令处理本地上传的照片。



![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd61713434271.jpg)



8.点击完成！

![img](https://cdn.jsdelivr.net/gh/misu198/Midjourney@main/guge/swapd71713434166.jpg)



9. 请注意，``INSwapper`` 上下文菜单也可以处理用户在您的 Discord 频道中上传的图像。



 🙀 其他注意事项 

1您可以使用/listid命令列出所有已注册的 ID。注册的ID总数不能超过10个，也可以使用/delid和/delall命令删除注册的ID。

2注册的ID名称只能是字母和数字，不能超过8个字符。

3对于多面替换，可以输入一个逗号分割的idname列表，比如/setid me,you,him,her

4您可以通过使用相同的 ID 名称重新上传来覆盖旧的 ID 功能。

5正视、高画质、无眼镜、无厚重刘海证件照优先。

6如果不想上传证件照，可以使用insightface python包生成自己的人脸证件特征，保存为.npy文件，其中shape=(512,)，用于上传。

7每个 Discord 帐户每天可以执行 50 个命令以避免自动脚本。

8这是在早期开发阶段，所以我们不能保证在每种情况下都会有很好的结果。

9请仅将其用于个人娱乐目的。

10如果有任何问题，请加入我们的 Discord 群组：[链接](https://discord.gg/65Ma47ymPc)