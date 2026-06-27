# 极简工具箱

纯前端在线工具集合，单文件实现，零依赖。

## 工具列表

| 工具 | 说明 |
|------|------|
| JSON 格式化 | 格式化、压缩、校验 JSON 数据 |
| 文本对比 | 逐行 diff，高亮新增/删除 |
| Base64 编解码 | 文本与 Base64 互转 |
| 时间戳转换 | Unix 时间戳与日期互转 |
| 正则测试 | 实时正则表达式匹配 |
| Markdown 预览 | 实时渲染 Markdown |
| 颜色转换 | HEX / RGB / HSL 互转 |
| 字数统计 | 字数、字符、行数、段落、阅读时间 |

## 技术栈

- 纯 HTML / CSS / JavaScript，无框架依赖
- 单文件部署（`index.html`）
- 暗色主题，响应式布局，移动端适配
- 数据本地处理，不上传服务器

## 部署

任意静态托管平台均可：

```bash
# Vercel
npx vercel --prod

# Netlify
netlify deploy --prod --dir .

# GitHub Pages
# 推送到 GitHub 仓库后在 Settings > Pages 中启用
```

## 本地运行

直接在浏览器中打开 `index.html`，或使用任意 HTTP 服务器：

```bash
python -m http.server 8080
# 访问 http://localhost:8080
```

## 安全说明

- 所有用户输入在拼接 innerHTML 前经过 `esc()` 转义（`&`, `<`, `>`, `"`, `'`）
- 纯前端运行，无后端接口，无第三方请求
