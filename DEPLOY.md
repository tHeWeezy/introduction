# GitHub Pages 部署指南

## 步骤 1：准备文件

将以下文件放在同一个文件夹中：

### HTML 文件
- `index.html`（将 `beer-bash-intro.html` 重命名为 `index.html`）

### 图片文件
- `个人照片.jpg`
- `头像.jpg`
- `dj.jpg`
- `唱片收藏.jpeg`
- `近期买的一些唱片.jpg`
- `陶喆唱片.png`
- `唱片黑胶.jpeg`
- `kanye01.JPG`
- `kanye02.jpg`
- `bettercall saul.jpeg`
- `法拉利01.PNG`
- `法拉利02.JPG`
- `xj01.jpg` ~ `xj09.jpg`（9张新疆照片）

## 步骤 2：创建 GitHub 仓库

1. 登录 GitHub (https://github.com)
2. 点击右上角 "+" → "New repository"
3. 仓库名称：`beer-bash-intro`（或任意名称）
4. 设置为 **Public**
5. 点击 "Create repository"

## 步骤 3：上传文件

### 方法 A：网页上传（最简单）

1. 在新创建的仓库页面，点击 "uploading an existing file"
2. 将所有文件（HTML + 图片）拖拽到页面
3. 点击 "Commit changes"

### 方法 B：使用 Git 命令

```bash
# 在你的文件夹中打开终端
cd /path/to/your/folder

# 初始化 Git
git init

# 添加所有文件
git add .

# 提交
git commit -m "Initial commit"

# 关联远程仓库（替换成你的用户名和仓库名）
git remote add origin https://github.com/你的用户名/beer-bash-intro.git

# 推送
git branch -M main
git push -u origin main
```

## 步骤 4：启用 GitHub Pages

1. 进入仓库页面
2. 点击 "Settings"（设置）
3. 左侧菜单找到 "Pages"
4. 在 "Source" 下拉菜单中选择 `main` 分支
5. 点击 "Save"
6. 等待几分钟，页面会显示你的网站链接：
   ```
   https://你的用户名.github.io/beer-bash-intro/
   ```

## 步骤 5：访问和演讲

- 在任何电脑的浏览器中打开上面的链接
- 按 F11 进入全屏模式
- 使用鼠标滚轮或上下箭头键切换页面
- 点击右侧导航点快速跳转

## 更新内容

如果需要修改内容：
1. 修改本地文件
2. 重新上传到 GitHub（覆盖原文件）
3. 等待几分钟自动更新

## 注意事项

- 确保所有图片文件名与 HTML 中引用的完全一致（包括大小写）
- 首次部署可能需要 5-10 分钟生效
- 链接可以分享给任何人访问
