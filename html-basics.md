# HTML 基础标签入门

**适用人群**: 零基础新手
**学习目标**: 掌握 HTML 最常用的三个基础标签：标题 (h1~h6)、段落 (p)、超链接 (a)

---

## 开场白

你好！欢迎来到 HTML 基础标签入门课程。我是你的编程学习伙伴。

在这门课程中，我们将学习 HTML 最基础也是最重要的三个标签：
- **h1~h6** - 标题标签
- **p** - 段落标签
- **a** - 超链接标签

准备好了吗？我们开始吧！

---

## 第一部分：标题标签 (h1~h6)

### 语法讲解

HTML 有 6 个级别的标题标签，从 `<h1>` 到 `<h6>`：

```html
<h1>一级标题 - 最大最重要的标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题 - 最小最不重要的标题</h6>
```

### 核心要点

| 标签 | 字号大小 | 使用场景 |
|------|----------|----------|
| h1 | 最大 | 页面主标题，每页只用一个 |
| h2 | 次大 | 主要章节标题 |
| h3 | 中等 | 子章节标题 |
| h4-h6 | 递减 | 更细分的内容层级 |

### 完整示例

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>标题标签示例</title>
</head>
<body>
    <h1>欢迎来到我的博客</h1>
    <h2>第一篇：HTML 学习之旅</h2>
    <h3>1.1 为什么要学习 HTML</h3>
    <h4>1.1.1 HTML 是网页的基础</h4>
    <h5>补充说明</h5>
    <h6>页脚信息</h6>
</body>
</html>
```

### 使用场景示例

```html
<!-- 新闻网站结构 -->
<h1>今日头条新闻</h1>        <!-- 网站名称 -->
<h2>国内新闻</h2>            <!-- 新闻分类 -->
<h3>经济发展新政策发布</h3>   <!-- 具体新闻标题 -->

<!-- 博客文章结构 -->
<h1>我的编程学习日记</h1>     <!-- 博客主标题 -->
<h2>第一章：HTML 入门</h2>    <!-- 文章标题 -->
<h3>什么是 HTML</h3>         <!-- 小节标题 -->
```

---

## 第二部分：段落标签 (p)

### 语法讲解

`<p>` 标签用于定义文本段落：

```html
<p>这是第一段文字内容。</p>
<p>这是第二段文字内容。</p>
<p>这是第三段文字内容。</p>
```

### 核心要点

- 每个 `<p>` 标签会自动在前后添加间距
- 段落内的换行需要用 `<br>` 标签
- 不能直接在段落内写另一个 `<p>` 标签

### 完整示例

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>段落标签示例</title>
</head>
<body>
    <h1>关于我</h1>
    
    <p>你好！我是一名前端开发爱好者。</p>
    
    <p>我喜欢探索新技术，尤其是 JavaScript 和 React。</p>
    
    <p>这个网站是我分享学习心得的地方。</p>
    
    <h2>我的编程经历</h2>
    
    <p>2024 年，我开始学习编程。<br>
    起初我觉得很难，但坚持下来后发现越来越有趣。<br>
    现在我已经能做出自己的网页了！</p>
</body>
</html>
```

---

## 第三部分：超链接标签 (a)

### 语法讲解

`<a>` 标签用于创建超链接，最重要的属性是 `href`：

```html
<a href="https://www.example.com">点击这里访问示例网站</a>
```

### 常用属性

| 属性 | 说明 | 示例 |
|------|------|------|
| href | 链接地址（必需） | `href="https://example.com"` |
| target | 打开方式 | `target="_blank"` 新标签页打开 |
| title | 鼠标悬停提示 | `title="点击查看详情"` |
| name/id | 锚点定位 | `name="top"` 或 `id="top"` |

### 完整示例

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>超链接标签示例</title>
</head>
<body>
    <h1>常用网站推荐</h1>
    
    <h2>学习资源</h2>
    <p>
        <a href="https://developer.mozilla.org/zh-CN/" target="_blank" title="MDN Web 文档">
            MDN Web 文档 - 最权威的前端学习资料
        </a>
    </p>
    
    <p>
        <a href="https://github.com" target="_blank">GitHub - 代码托管平台</a>
    </p>
    
    <h2>页面内跳转</h2>
    <p><a href="#section1">跳转到第一节</a></p>
    <p><a href="#section2">跳转到第二节</a></p>
    <p><a href="#top">回到顶部</a></p>
    
    <h2 id="section1">第一节内容</h2>
    <p>这里是第一节的内容...</p>
    
    <h2 id="section2">第二节内容</h2>
    <p>这里是第二节的内容...</p>
    
    <p id="top">页面底部 - 可以点"回到顶部"返回</p>
</body>
</html>
```

---

## 综合练习：制作一个简单的个人页面

把学到的三个标签组合起来：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>我的个人主页</title>
</head>
<body>
    <h1>张三的个人主页</h1>
    
    <h2>关于我</h2>
    <p>大家好，我叫张三，是一名大学生。</p>
    <p>我热爱编程，正在学习 Web 开发技术。</p>
    
    <h2>我的兴趣</h2>
    <p>除了编程，我还喜欢摄影和阅读。</p>
    
    <h2>联系我</h2>
    <p>
        邮箱：<a href="mailto:zhangsan@example.com">zhangsan@example.com</a><br>
        GitHub：<a href="https://github.com/zhangsan" target="_blank">@zhangsan</a>
    </p>
    
    <h2>推荐资源</h2>
    <p>
        <a href="https://developer.mozilla.org/zh-CN/" target="_blank" title="MDN 文档">
            学习 Web 开发，推荐访问 MDN 文档
        </a>
    </p>
</body>
</html>
```

---

## 学习检查清单

完成本课程后，你应该能够：

- [ ] 说出 h1~h6 的区别和使用场景
- [ ] 用 `<p>` 标签组织段落内容
- [ ] 创建指向外部网站的链接
- [ ] 创建页面内的锚点跳转
- [ ] 组合三个标签制作简单页面

---

## 互动练习

现在，试着回答以下问题：

**问题 1**: 一个网页应该有几个 `<h1>` 标签？

**问题 2**: 如何让链接在新标签页中打开？

**问题 3**: 写一个完整的 HTML 页面，包含：
- 一个主标题
- 两个二级标题
- 至少两个段落
- 一个指向百度 (https://www.baidu.com) 的链接

---

如果你有任何问题，随时问我！我们可以一起讨论和练习。
