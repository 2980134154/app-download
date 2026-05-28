# 首创京都期货 - 应用下载页面

这是一个自动检测设备类型并跳转到对应应用商店的 H5 页面。

## 功能特性

- ✅ 自动检测 iOS/Android 设备
- ✅ 2秒倒计时后自动跳转
- ✅ 支持手动点击按钮跳转
- ✅ 响应式设计，适配各种屏幕
- ✅ 支持微信内置浏览器
- ✅ 美观的渐变色 UI 设计

## 部署到 GitHub Pages

### 方法 1：通过 GitHub 网页操作

1. 在 GitHub 上创建一个新仓库（例如：`app-download`）
2. 上传 `index.html` 文件到仓库根目录
3. 进入仓库的 Settings > Pages
4. 在 "Source" 下选择 `main` 分支
5. 点击 Save
6. 等待几分钟后，访问 `https://你的用户名.github.io/仓库名/`

### 方法 2：通过命令行操作

```bash
# 进入项目目录
cd "/Users/tsharing/Documents/h5 跳转商店"

# 初始化 Git 仓库
git init

# 添加文件
git add .

# 提交
git commit -m "Initial commit: 添加应用下载页面"

# 关联远程仓库（替换成你的仓库地址）
git remote add origin https://github.com/你的用户名/仓库名.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

然后在 GitHub 仓库设置中启用 Pages。

## 修改链接

如果需要修改 Android 下载链接，编辑 `index.html` 文件中的配置：

```javascript
const CONFIG = {
    iosUrl: 'https://apps.apple.com/cn/app/%E9%A6%96%E5%88%9B%E4%BA%AC%E9%83%BD%E6%9C%9F%E8%B4%A7/id1439870586',
    androidUrl: '你的新链接', // 修改这里
    autoRedirectDelay: 2000 // 自动跳转延迟时间（毫秒）
};
```

## 本地测试

直接用浏览器打开 `index.html` 文件即可预览效果。

## 技术栈

- 纯 HTML + CSS + JavaScript
- 无需任何框架或依赖
- 兼容所有现代浏览器
