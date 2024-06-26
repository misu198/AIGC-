# 技巧七：多参数同时使用
---
在使用 img2img 的方法生成头像时，我发现问题是「文字权重比图片权重高」，导致其生成的图片不像原图，iw 参数在 V5 里最多提升图片权重到 2，所以我就在想有没有可能进一步降低文字的权重。

然后我就试了下 s 参数，发现的确好了很多。

如果生成的图片还是不像，你可以在 —iw 2 基础上，再加一个参数 —s 200 ，注意同时用两个参数时，中间不要有逗号。我发现加了 s 参数之后的确像了很多，我个人猜测是 s 和 iw 连用会进步一削弱 text 的权重。

s 是控制生成图片的风格化程度。简单理解，这个值越低会更符合 text prompt 的描述，数值越高艺术性就会越强，但跟 text prompt 关联性就会比较弱。所以如果你生成的图还是不像，就加大这个值，比如调到 500。

我想通过这个案例告诉大家，多个参数一起使用，有可能会形成合力，进一步放大模型的能力。未来有新的参数能力，不妨也想想有没有可能一起用？