# GitHub Pages 发布包

这个目录已经整理成可直接发布到 GitHub Pages 的静态站点。

## 目录结构

```text
github-pages-site/
  index.html
  .nojekyll
  assets/
    showcase/
      login-screen.png
      customer-screen.png
      workspace-screen.png
      knowledge-screen.png
      analytics-screen.png
```

## 直接发布到 GitHub Pages

1. 在 GitHub 新建一个公开仓库，例如 `luminaire-portfolio`
2. 打开这个目录，把里面的全部文件上传到仓库根目录
3. 在仓库页面进入 `Settings -> Pages`
4. 在 `Build and deployment` 中选择：
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/(root)`
5. 保存后等待 1 到 3 分钟
6. 访问生成的链接：

```text
https://你的用户名.github.io/luminaire-portfolio/
```

## 本地预览

直接双击 `index.html`，或者在 PowerShell 里运行：

```powershell
Invoke-Item .\index.html
```

## 注意

- 当前页面仍使用 Tailwind CDN、Chart.js CDN 和 Google Fonts。
- 大多数情况下 GitHub Pages 展示会和本地基本一致。
- 如果你后面想追求更稳定的一致性，可以再做一版“无 CDN 发布版”。
