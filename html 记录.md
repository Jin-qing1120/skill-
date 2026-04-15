---
name: "js-practice-helper"
description: "帮助完成JavaScript基础知识练习，生成包含JavaScript代码的HTML页面，并使用skill推送仓库到GitHub。Invoke when user needs to complete JavaScript basic knowledge exercises and push to GitHub."
---

# JavaScript Practice Helper

## 功能

- 生成包含JavaScript基础知识练习的HTML页面
- 涵盖变量定义、变量类型、表达式、流程控制、函数等内容
- 提供代码示例和练习
- 帮助将作业推送到GitHub仓库

## 使用方法

1. 调用此skill创建JavaScript练习HTML文件
2. 编辑文件内容，添加你的JavaScript代码练习
3. 使用skill将仓库推送到GitHub
4. 提交commit记录作为作业提交

## 示例HTML结构

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript基础知识练习</title>
</head>
<body>
    <h1>JavaScript基础知识练习</h1>
    
    <script>
        // 变量定义
        let name = "JavaScript";
        const version = 1.0;
        var age = 25;
        
        // 变量类型
        console.log(typeof name); // string
        console.log(typeof version); // number
        console.log(typeof age); // number
        
        // 表达式
        let sum = 10 + 5;
        let product = 10 * 5;
        console.log("Sum:", sum);
        console.log("Product:", product);
        
        // 流程控制
        if (sum > 10) {
            console.log("Sum is greater than 10");
        } else {
            console.log("Sum is less than or equal to 10");
        }
        
        // 函数
        function greet(name) {
            return "Hello, " + name + "!";
        }
        
        console.log(greet("World"));
    </script>
</body>
</html>
```

## 推送到GitHub

使用skill的推送功能将仓库推送到GitHub，并获取commit记录作为作业提交。