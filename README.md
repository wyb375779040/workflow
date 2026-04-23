# GitHub Pages 发布说明

这个目录已经整理成可直接发布到 GitHub Pages 的静态站点。

## 文件说明

- `index.html`：站点首页
- `.nojekyll`：关闭 Jekyll 处理，按纯静态文件发布

## 最短发布方式

1. 在 GitHub 新建一个公开仓库，例如 `ai-product-workflow`
2. 把这个目录里的文件上传到仓库根目录
3. 进入 GitHub 仓库
4. 打开 `Settings -> Pages`
5. 在 `Build and deployment` 里选择：
   - `Source = Deploy from a branch`
   - `Branch = main`
   - `Folder = / (root)`
6. 保存后等待 GitHub Pages 发布完成

发布后地址通常类似：

`https://你的用户名.github.io/ai-product-workflow/`

## 本地命令行方式

```bash
cd "Ai PMLX/产品技术ClaudeCode协作模式/github-pages"
git init
git add .
git commit -m "init github pages site"
git branch -M main
git remote add origin git@github.com:你的用户名/ai-product-workflow.git
git push -u origin main
```

## 说明

- 如果要让所有人都能直接访问，仓库建议设为 `public`
- GitHub Pages 适合放静态 HTML、CSS、JS，不适合放敏感信息
