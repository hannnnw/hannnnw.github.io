# 汪晗的个人作品集 (Wang Han's Portfolio)

这是一个可以直接部署到 GitHub Pages 的静态个人作品集网页，展示教育背景与实习经历。

## 项目特点

- **零依赖**：无需安装 Node.js、npm 或任何构建工具。
- **单文件部署**：只有一个 `index.html`，上传到 GitHub 后即可部署。
- **简约专业设计**：使用现代无衬线字体 (Inter & Noto Sans SC)，配色干净、布局清晰。
- **中英双语支持**：一键切换中文和英文界面。
- **响应式布局**：适配手机、平板和桌面端。
- **动态交互**：点击实习经历卡片可展开/收起项目细节。

## 文件结构

```text
portfolio-github/
├── index.html   # 页面结构、样式和交互逻辑都在这个文件中
└── README.md    # GitHub Pages 部署说明
```

## 如何在 GitHub Pages 上部署

### 方法一：通过 GitHub 网页上传

1. 登录 GitHub。
2. 点击右上角 **+** → **New repository**。
3. 创建一个公开仓库，例如：`portfolio`。
4. 上传本文件夹中的 `index.html` 和 `README.md` 到仓库根目录。
5. 进入仓库 **Settings** → **Pages**。
6. 在 **Build and deployment** 中选择：
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
7. 点击 **Save**。
8. 等待几分钟后，即可通过类似下面的链接访问：

```text
https://你的GitHub用户名.github.io/portfolio/
```

### 方法二：通过 Git 命令上传

```bash
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/你的GitHub用户名/portfolio.git
git push -u origin main
```

然后按上面的方法在 GitHub 仓库设置中开启 GitHub Pages。

## 如何修改内容

直接打开 `index.html`，搜索以下字段即可修改：

- `eduData`：教育背景。
- `data`：实习经历与项目详情。
- `i18n`：页面标题、按钮、提示文案等中英文内容。

## 技术栈

- HTML5
- CSS3
- Vanilla JavaScript
