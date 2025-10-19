# Hexo 黑猫 Live2D 包

这是一个 Hexo 博客资源包，包含黑猫 Live2D 模型和示例背景图。

## 使用方法
1. 将 \`source/\` 目录放到 Hexo 项目根目录。
2. 在 CSS 中添加:
\`\`\`css
body {
    background-image: url("/images/my-bg.jpg");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
}
\`\`\`
3. 在 footer.ejs 添加:
\`\`\`html
<script src="https://unpkg.com/live2d-widget@latest/lib/L2Dwidget.min.js"></script>
<script>
L2Dwidget.init({
    model: { jsonPath: "/live2d/blackcat/model.json" },
    display: { position: "right", width: 150, height: 300 },
    mobile: { show: true },
    log: false
});
</script>
\`\`\`
