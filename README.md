# reveal.js academic template

把 `index.html`、`slides.md`、`custom.css` 放到 reveal.js 根目录（与 `dist/`、`plugin/` 同级）。

## 运行
```bash
python -m http.server 8000
```

然后打开：

```text
http://localhost:8000/index.html
```

## 维护方式
- 以后主要只改 `slides.md`
- 样式改 `custom.css`
- 数学公式配置在 `index.html`

## 约定
- `---` 表示下一页
- `--` 表示竖向下一页（当前文件暂未使用）
- `Note:` 开头的内容会被 reveal.js 当作 speaker notes
- 复杂公式建议继续使用这种稳定写法：

```md
<div class="math-block">\[
\bm{z} \rightarrow \bm{c}_{k^*}
\]</div>
```
