# 我的第一个网页

一个用 HTML、CSS 和 JavaScript 写的静态网页小示例。页面中央有一张卡片，点击按钮后，卡片里的文字会变成另一句话。

## 功能

- 展示一张居中的卡片，包含标题和一段说明文字
- 点击「点我试试」按钮，通过 JavaScript 修改页面文字

## 文件结构

```
.
├── index.html    # 页面结构
├── style.css     # 页面样式
└── script.js     # 交互逻辑
```

## 如何运行

这是一个纯静态页面，不需要安装任何依赖。

1. 下载或克隆本仓库到本地
2. 直接用浏览器打开 `index.html` 即可

也可以用本地服务器打开（可选）：

```bash
# Python 3
python -m http.server 8000

# 然后访问 http://localhost:8000
```

## 代码说明

**index.html**

定义了页面结构：一个 `card` 容器，里面有标题、一段带 `id="msg"` 的文字，以及一个绑定 `changeText()` 的按钮。同时引入了 `style.css` 和 `script.js`。

**style.css**

负责页面外观：用 Flexbox 让卡片在页面中水平垂直居中，给卡片加了白底、圆角和阴影，并设置了按钮的悬停变色效果。

**script.js**

只做一件事：定义 `changeText()` 函数，把 `id="msg"` 元素的文字替换成「你刚刚触发了一段 JavaScript。」。

## 可以继续尝试的方向

- 让按钮点击后在两句文字之间来回切换
- 增加一个输入框，把用户输入的内容显示到页面上
- 给卡片加一个淡入动画
- 把文字内容改成从数组里随机抽取

## 许可

本项目仅用于学习示例，可自由使用和修改。
```

你可以直接把上面内容保存为 `README.md`，然后提交推送：

```bash
git add README.md
git commit -m "add README"
git push
```
