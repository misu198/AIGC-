# Docsify开放课程入门工具包（Docsify Open Course Starter Kit）

[![Docsify](https://img.shields.io/npm/v/docsify?label=docsify)](https://docsify.js.org/)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/hibbitts-design/docsify-open-course-starter-kit/blob/main/LICENSE)
<a href="https://discord.gg/zT8eS8ZG">
    <img src="https://img.shields.io/badge/chat-on%20discord-7289DA.svg" alt="Docsify Discord Chat" />
</a>

> 这是一个快速创建基于 Markdown 的开放式课程网站的入门套件，使用网站生成器 [Docsify](https://docsify.js.org)。全局导航元素可以隐藏，以便将页面无缝嵌入到学习管理系统 (LMS) 中。还包括一个可选的 "编辑此页面" 链接。.


🚀 GitHub 页面快速入门
---
**前飞行检查清单**

1. GitHub 账户

**安装和部署**

1. 在源仓库上点击 **使用此模板**（右上角的绿色按钮），然后选择 **创建一个新仓库**
![Docsify 开放课程入门套件 - 安装页面 1](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-install-1.png)

2. 为您的新仓库选择一个名称，用于存放复制的站点文件，然后点击 **从模板创建仓库**
![Docsify 开放课程入门套件 - 安装页面 2](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-install-2.png)

3. 进入您新创建的仓库的 **设置**，点击 **Pages** 标签（在左侧），选择 **main 分支**，然后选择 **docs 文件夹**，最后点击 **保存** 按钮（更多细节请参阅 [Docsify 文档](https://docsify.js.org/#/deploy?id=github-pages)）
![Docsify 开放课程入门套件 - 安装页面 3](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-install-3.png)

4. 完成！（使用 **Pages** 标签上提供的 URL 查看您的新站点 - 您的站点最初可用需要最多 10 分钟）
![Docsify 开放课程入门套件 - 安装页面 4](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-install-4.png)

您使用 GitLab 吗？您也可以使用 [GitLab Pages](https://docsify.js.org/#/deploy?id=gitlab-pages) 配合 Docsify！
---  

1. 打开您要编辑的存储库中 `docs` 文件夹中的 Docsify Markdown (.md) 页面
![编辑您的 Docsify 网站页面 1](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-page-edit-1.png)

2. 点击 **铅笔图标**（位于左上角的工具栏区域）开始编辑
![编辑您的 Docsify 网站页面 2](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-page-edit-2.png)

3. 滚动到页面底部，点击 **提交更改** 按钮以保存您的更改
![编辑您的 Docsify 网站页面 3](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-page-edit-3.png)

[了解更多关于在 Docsify 中创建页面的信息。](https://docsify.js.org/#/more-pages)

🔗 激活您的 Docsify 网站上的 “编辑此页面” 链接
---   

💻 在本地编辑您的 Docsify 网站页面

1. 在您的 GitHub 存储库的顶层复制 URL
![Docsify 开放课程入门套件 - “编辑此页面” 链接 1](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-gitlink-1.png)

2. 点击 **docs** 文件夹
![Docsify 开放课程入门套件 - “编辑此页面” 链接 2](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-gitlink-2.png)

3. 点击 **index.html** 文件
![Docsify 开放课程入门套件 - “编辑此页面” 链接 3](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-gitlink-3.png)

4. 点击 **铅笔图标**（位于左上角的工具栏区域）开始编辑
![Docsify 开放课程入门套件 - “编辑此页面” 链接 4](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-gitlink-4.png)

5. 找到行 `var gitLinkRepoURL = '';`，在两个引号之间输入您自己的 GitHub 存储库的 URL（将 `github.com` 替换为 `github.dev` 可以使用目前处于 Beta 阶段的 GitHub.dev 在线编辑器），然后滚动到页面底部并点击 **提交更改** 按钮以保存您的更改
![Docsify 开放课程入门套件 - “编辑此页面” 链接 5](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-gitlink-5.png)
---  

您可以在桌面上编辑您的 Docsify 网站页面：

1. 点击您存储库上的 **Code**（右上角的绿色按钮）。
2. 选择 **Open Desktop** 并按照提示操作，如果尚未安装 [GitHub Desktop](https://desktop.github.com/)，请先安装。
3. 现在您可以使用您选择的桌面编辑器（例如 [Atom](https://atom.io/)）编辑您的 Docsify 网站（在 `docs` 文件夹中）。
4. 使用 GitHub Desktop 将任何更改推送到您的存储库。

[了解更多关于使用 GitHub Desktop](https://help.github.com/en/desktop/contributing-to-projects/committing-and-reviewing-changes-to-your-project)。

您也可以克隆（即下载）您存储库的副本到您的计算机上，并 [本地运行 Docsify](https://docsify.js.org/#/quickstart) 预览您的网站。请参考下面的视频了解详情。

🧩 将您的 Docsify 页面内容嵌入其他系统

![将 Docsify 开放课程页面嵌入到 Canvas LMS](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/docsify-oc-canvas.png)
_图 2. 将 Docsify 开放课程页面嵌入到 Canvas LMS。探索一个使用 Docsify 开放课程页面作为内容的示例 Canvas LMS 课程，网址为 [https://canvas.sfu.ca/courses/44038/](https://canvas.sfu.ca/courses/44038)_

可选的 `embedded`（全小写）URL 参数可以隐藏网站的侧边栏，实现将 Docsify 页面内容无缝嵌入到其他平台中，例如 Canvas LMS、Moodle、Microsoft Teams，或者在现有或新的浏览器标签中显示。参数 `standalone` 可以作为 `embedded` 的别名使用。

要仅显示 Docsify 页面内容，请在 Docsify 页面 URL 中添加以下内容：

`?embedded=true`

示例标准的 Docsify 页面：  
https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources  

示例显示仅页面内容的 Docsify 页面（即不显示侧边栏）：  
https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true  

要可选显示页面目录（基于包含的标题），请使用以下内容：

`?embedded=true&toc=true`

示例显示仅页面内容的 Docsify 页面：  
https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true  

示例显示仅页面内容且包含页面目录的 Docsify 页面：  
https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&toc=true  

要可选覆盖显示仅页面内容时隐藏导航栏的设置，请使用以下内容：

`?embedded=true&navbar=true`

示例显示仅页面内容的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true)  

示例显示仅页面内容且仍显示导航栏的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&navbar=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&navbar=true)  

要可选隐藏 "编辑此页面" 链接，请使用以下内容：

`?embedded=true&hidegitlink=true`

示例显示仅页面内容的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true)  

示例显示仅页面内容且隐藏 "编辑此页面" 链接的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&hidegitlink=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&hidegitlink=true)  

要可选显示页脚（'_footer.md' 文件），请使用以下内容：

`?embedded=true&footer=true`

示例不显示页脚的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true)  

示例显示页脚的 Docsify 页面：  
[https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&footer=true](https://hibbitts-design.github.io/demo-docsify-open-course-starter-kit/#/resources?embedded=true&footer=true)  

🖼 将您的 Docsify 页面内容呈现为独立的网页

除了在将 Docsify 页面内容嵌入其他系统时使用 URL 参数外，还可以永久将所有页面显示为独立页面，并始终显示页面目录。

**显示所有页面为独立页面**
1. 打开 `index.html` 文件进行编辑。
2. 找到行 `var standalone = false;`，将其更改为 `var standalone = true;`。
3. 保存 `index.html` 文件并重新加载站点。

**显示页面目录**
1. 打开 `index.html` 文件进行编辑。
2. 找到行 `var ToC = false;`，将其更改为 `var showToC = true;`。
3. 保存 `index.html` 文件并重新加载站点。

请注意，页面必须具有一系列标题 (#, ##, ###) 才能正确显示目录。

❛❜ 设置您的 Docsify 网站名称
---  

🛠 使用 LMS 托管 Docsify 开放课程网站

由于 Docsify 开放课程入门套件不需要 web 服务器，实际上它可以托管在许多支持文件库的 LMS 中，如 Canvas 和 Moodle。

例如，这是一个 [在 Canvas 课程中托管的 Docsify 开放课程网站](https://canvas.sfu.ca/courses/44038/files/15884796/download)。在同一系统中托管的单个 Docsify 开放课程网站页面也可以嵌入。

**在您的 LMS 上托管 Docsify 开放课程网站**
1. 点击您存储库页面上的 **下载** 按钮。
2. 将文件上传到您的 LMS 文件存储区，并解压上传的文件。
3. 根据您的 LMS，确定加载 Docsify `Docs` 文件夹中的 `index.html` 文件所需的外部 URL。在 Canvas 中，示例 URL 可能类似于 `https://canvas.sfu.ca/courses/44038/files/15884796/download`。

| :warning: | 一旦在您的 LMS 中托管，对源 GitHub 存储库进行的更改不会自动反映在您托管的 Docsify 网站上。任何 GitHub 存储库的更新都必须手动上传到 LMS 文件库区域。 |
|---|:--|

📚 Docsify 和 Markdown 资源
---
**Docsify**  
[Docsify 文档](https://docsify.js.org/#/?id=docsifyg)  
[MichaelCurrin 的 Docsify 基础教程](https://michaelcurrin.github.io/docsify-js-tutorial/#/?id=docsify-basics)  

**Docsify 主题**  
[Docsify Themeable 文档](https://jhildenbiddle.github.io/docsify-themeable/#/introduction)  
[Docsify Themeable GitHub](https://github.com/jhildenbiddle/docsify-themeable)  

**Markdown**  
[Markdown Here 备忘表](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)  
[Markdown 指南](https://www.markdownguide.org/)  

🧰 有用的 Markdown CSS 类
---

`accordion`

```html
<div class="accordion">

<details>
  <summary>主题一</summary>
  
  主题一的详细内容在这里。
  
</details>

<details>
  <summary>主题二</summary>
  
  主题二的详细内容在这里。
  
</details>

</div>
```

`badge`  

```html
<span class='badge'> Tue Jun 12th 11:59pm PDT</span>
```

```html
<span class='badge' style='--badge-bg-color: #0164db;'> Tue Jun 12th 11:59pm PDT</span>
```

```html
<span class='badge' style='--badge-bg-color: #e7c500; --badge-text-color: #000;'> Tue Jun 12th 11:59pm PDT</span>
```

```html
<span class='badge'> [Tue May 16 2:30pm PT](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CMPT-363+Blackboard+Mini-lectures+and+Activities&iso=20220516T1430&p1=256&ah=1&am=50)</span>  
```

`banner-image` (cropped to height of 250px on large screens, 125px on small screens)  

```markdown
![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-image')
```

`banner-tall-image` (cropped to height of 350px on large screens, 175px on small screens)  

```markdown
![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-tall-image')
```

`button`  

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')
```

`button-rounded`  

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button-rounded')
```

`button-secondary`  

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button-secondary')
```

`button-rounded-secondary`  

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button-rounded-secondary')
```

`embedly-card` (for linked article previews, embedded slides/videos, etc.)  

```markdown
<a class="embedly-card" data-card-controls="0" data-card-align="left" href="https://blog.prototypr.io/defining-usability-e7bf42e8abd0">Defining usability</a>
```

`header-image-fade` (suggested width of 1200px to 2000px)  

```markdown
![Photo of Mountain](images/mountain.jpg ':class=header-image-fade')
```

`header-image-fade-full-width` (suggested size of 1200px to 2000px, and display of Table of Contents is not available)  

```markdown
![Photo of Mountain](images/mountain.jpg ':class=header-image-fade-full-width')
```

`header-image-full-width` (suggested size of 1200px to 2000px width and 400px to 600px height, and display of Table of Contents is not available)  

```markdown
![Photo of Mountain](images/mountain.jpg ':class=header-image')
```

`image-75` (scale image to 75%)

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-75')
```

`image-50` (scale image to 50%)

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-50')
```

`image-25` (scale image to 25%)

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-25')
```

`image-75-border`

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-75-border')
```

`image-50-border`

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-50-border')
```

`image-25-border`

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-25-border')
```

`image-border`

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-border')
```

`image-border-rounded`

```markdown
![Photo of Mountain](images/mountain.jpg ':class=image-border-rounded')
```

`navpill`

```markdown
[GitHub](https://github.com/hibbitts-design/docsify-this ':class=navpill')
```

```html
<a class="navpill" href="https://github.com" target="_blank"><i class="fab fa-github fa-fw"></i>GitHub</a>
```

`row` & `column`  

```html
<div class="row">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

```html
<div class="row reverse-columns">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

```html
<div class="row">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column-right">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

`video-container-4by3`  

```html
<div class="video-container-4by3"><div class="video-container-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/lJIrF4YjHfQ"></iframe></div>
```

`video-container-16by9`  
Automatically added to all iFrames with the source domains 'youtube.com' or 'docs.google.com'.  
```html
<div class="video-container-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/lJIrF4YjHfQ"></iframe></div>
```

🎨 视觉定制
---

可以使用位于 `docs/assets/css` 文件夹中的 `custom.css` 文件在 Docsify 开放课程入门套件网站中进行视觉定制。在这个文件中可以定义新的 Markdown CSS 类。

CSS：
```css
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
```

Markdown：
```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=mybutton')
```

还可以配置 [Docsify Themeable 的 CSS 设置](https://jhildenbiddle.github.io/docsify-themeable/#/customization?id=base)，如默认的 `custom.css` 文件中所示的示例。

CSS：
```css
:root {
    --link-color: #0F6CBF!important;
}
```

还可以配置双重 CSS 样式，其中 CSS 应用于查看网站时（包含在 `_sidebar.md` 文件中的覆盖自定义 CSS 中）以及在查看独立页面（即 `?embedded=true`）时应用于 `custom.css` 文件中的其他 CSS 设置。

CSS in Sidebar file (`_sidebar.md`):  
```css
<style>
  :root {
    --link-color: #CC0633;
    --link-text-decoration: none;
    --link-text-decoration--hover: underline;
  }
</style>
```

🌐 使用 MAMP 在本地查看 Docsify 站点

另一种在本地查看 Docsify 站点的方法（如下所述）是使用 MAMP 在您自己的计算机上本地查看 Docsify 站点。

1. 下载 [MAMP](https://www.mamp.info/)
2. 将您的本地 Docsify 站点移动到 MAMP 的 **htdocs** 文件夹中
3. 启动 MAMP，点击 **WebStart**，然后点击 **My Website**
4. 点击包含您本地 Docsify 站点的文件夹，然后点击 **docs** 文件夹

📼 本地 Docsify 安装/配置的视频演示
---
[![Generating Documentation Sites with GitHub and Docsify - Alysson Alvaran](https://raw.githubusercontent.com/paulhibbitts/github-repo-images/master/youtube.png)](https://www.youtube.com/watch?v=TV88lp7egMw)  
_视频 1. 使用 GitHub 和 Docsify 生成文档站点 - Alysson Alvaran_

🙇‍ 感谢和特别鸣谢
---
[Docsify Themeable](https://github.com/jhildenbiddle/docsify-themeable)