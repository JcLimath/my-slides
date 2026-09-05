# My Slides

使用 Markdown 和 reveal.js 制作、通过 GitHub Pages 发布的在线演示文稿。

## 目录结构

```text
my-slides/
├─ dist/                 # reveal.js 公共核心文件
├─ plugin/               # reveal.js 公共插件
├─ custom.css            # 所有演示共用样式
├─ slides/
│  └─ mgno/
│     ├─ index.html      # 演示入口
│     ├─ slides.md       # Markdown 内容
│     ├─ images/         # 演示图片
│     └─ files/          # PDF 等附件
└─ index.html            # 演示列表首页
```

## 本地预览

在仓库根目录运行：

```powershell
py -m http.server 8000
```

然后访问：

```text
http://localhost:8000/
http://localhost:8000/slides/mgno/
```

外部 Markdown 需要通过 HTTP 服务器加载，不要直接双击 `index.html`。

## 新建演示

1. 复制 `slides/mgno/` 作为新演示目录。
2. 修改新目录中的 `index.html` 标题。
3. 编辑 `slides.md`。
4. 将图片放入 `images/`，在 Markdown 中使用 `images/example.png`。
5. 将 PDF 等附件放入 `files/`。

演示目录位于 `slides/<name>/` 两层路径下，因此公共 reveal.js 资源使用 `../../dist/`、`../../plugin/` 和 `../../custom.css`。

## Markdown 分页约定

- `---`：下一张横向幻灯片。
- `--`：当前幻灯片下方的竖向幻灯片。
- `Note:`：演讲者备注。

## 在线地址

- 演示列表：`https://jclimath.github.io/my-slides/`
- MGNO：`https://jclimath.github.io/my-slides/slides/mgno/`
