你好！欢迎来到失重的网络杂物间 (○｀∀´○)

是用来保存摘抄、网络书签以及其它一些文本类记录的地方（看中了搜索功能

`Last Update at 2024/9/6`

博客👉[匣](https://lunasa.icu/)

**关于**
- Start from 2024/3/26
- Docsify 搭建参考：
    - [Docsify 中文文档](https://docsify.js.org/#/zh-cn/)
    - [Docsify | 搭建个人静态笔记库](https://mantyke.icu/posts/2021/docsify-build/)
    - [B站视频教程：使用Docsify搭建笔记博客](https://www.bilibili.com/video/BV1kT4y1T7wY/)
    - [docsify的配置+全插件列表](https://xhhdd.cc/archives/80/comment-page-1)
    - [鱼’s Repository](https://note.gregueria.icu/#/README)
    - [呆’s 便利贴](https://doc.graugris.icu/#/about)
- 如有需要可以在主站点评论区留言！看到就会回复！

**备忘**
- 本地预览命令：`docsify serve docs`
- `!>` ：一段重要的内容
- `?>` ：普通提示
- 增加封面：在 `index.html` 中添加下方代码，然后在根目录下创建 ` _coverpage.md` 文件
```
<script>
    window.$docsify = {
      coverpage: true
    }
</script>
```
- `.nojekyll` 用于阻止 GitHub 仓库忽略掉下划线开头的文件
- 用 Obsidian 编辑的话要在文件夹下新建 `.gitignore` 并写入 `.obsidian`
- 在根目录下添加 `vercel.json` 并写入以下代码，可以直接输入子页面链接跳转，并且不会影响加载速度。
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

---
祝你开心 ^ ^
