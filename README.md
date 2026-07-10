# 深度用 AI · 内部培训网页

内部培训页面 —— 《深度用 AI:从提示词到闭环》。

基于 Claude Design Canvas（`.dc.html`）导出的静态页面，运行时由 `support.js`（React 客户端渲染）与 `image-slot.js` 提供，无需构建步骤。

## 本地预览

```bash
npx serve .
# 或
python -m http.server 8000
```

然后打开 http://localhost:8000

## 部署

纯静态站点，Vercel 直接部署根目录即可，无需构建命令。

## 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 页面本体（Design Canvas 模板 + 状态脚本） |
| `support.js` | Design Canvas 运行时（自动从 CDN 加载 React 并挂载） |
| `image-slot.js` | 图片占位槽组件 |
