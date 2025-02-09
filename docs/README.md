你好！欢迎来到失重的网络杂物间 (○｀∀´○)

是用来保存摘抄等文本类记录的地方（看中了搜索功能

`Last Update at 2024/9/6`

博客👉[匣](https://lunasa.icu/)

**关于**
- 建立于 2024/3/26
- Docsify 搭建参考：
    - [Docsify 中文文档](https://docsify.js.org/#/zh-cn/)
    - [Docsify | 搭建个人静态笔记库](https://mantyke.icu/posts/2021/docsify-build/)
    - [B站视频教程：使用Docsify搭建笔记博客](https://www.bilibili.com/video/BV1kT4y1T7wY/)
    - [docsify的配置+全插件列表](https://xhhdd.cc/archives/80/comment-page-1)
    - [鱼’s Repository](https://note.gregueria.icu/#/README)
    - [呆’s 便利贴](https://doc.graugris.icu/#/about)
- 如有需要可以在博客留言！看到就会回复！
- 祝你开心 ^ ^


**备忘**
- 本地预览命令：`docsify serve docs`
- `!>` ：一段重要的内容
- `?>` ：普通提示
- `.nojekyll` 用于阻止 GitHub 仓库忽略掉下划线开头的文件
- 用 Obsidian 编辑：在文件夹下新建 `.gitignore` 并写入 `.obsidian`
- 在根目录下添加 `vercel.json` 并写入以下代码，可以直接输入子页面链接跳转，并且不会影响加载速度。（by ChatGPT）
```
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ],
  "headers": [
    {
      "source": "/(.*).(js|css|png|jpg|svg|woff2)",
      "headers": [
        {
          "key": "Cache-Control",
          "value": "public, max-age=31536000, immutable"
        }
      ]
    }
  ]
}
```
- 配置步骤（也许有问题但上次是这么操作的
  1. 下载 node.js
  2. 命令行：`(sudo) npm i docsify. cli -g`
  3. `docsify init./docs`
  4. 网页 git 新建仓库，点击 `set in desktop`，跳到 github desktop，点击 clone
  5. 在 vercel import 仓库并 deploy
  6. 用 vscode 打开编辑 index.html 和 readme