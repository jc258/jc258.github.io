---
layout: post
title: "前端规范"
date: 2016-04-13 18:55:41
tags: [css, html, javascript, fed]
---

## HTML约定

1. 统一使用HTML5的标准文档类型：`<!DOCTYPE html>`
2. 在文档doctype申明之前，不允许加上任何非空字符；
3. 在调用外部CSS和JavaScript时，可以将type属性省略不写
4. 非必须属性值可以省略
    ```javascript
        //不建议
        <input type="text" readonly="readonly" />
        <input type="text" disabled="disabled" />

        //建议
        <input type="text" readonly />
        <input type="text" disabled />
    ```
5. 用双引号包裹属性值
6. 不允许非法的子元素嵌套。
    ```javascript
        //不建议
        <ul>
            <h3>列表标题</h3>
            <li>item 1</li>
            <li>item 2</li>
        </ul>

        //建议
        <div>
            <h3>列表标题</h3>
            <ul>
                <li>item 1</li>
                <li>item 2</li>
            </ul>
        </div>
    ```
7. 不推荐inline元素包含block元素；
8. 建议所有的标签闭合
9. 为img元素加上alt属性；
10. 为表单元素label加上for属性
11. 每个子元素都需要相对其父级缩进

## CSS约定

1. 一律使用link的方式调用外部样式
2. 不允许使用 style 属性写行内样式。
3. 建议使用英文进行样式命名，多单词使用中划线拼接
4. 书写格式
    - 选择器与大括号之间保留一个空格；
    - 冒号之后保留一个空格；
    - 逗号之后保留一个空格；
    - 所有规则需换行；
    - 多组选择器之间需换行。

    ```css
        //不建议
        main{
            display:inline-block;
        }
        h1,h2,h3{
            margin:0;
            background-color:rgba(0,0,0,.5);
        }
        //建议
        main {
            display: inline-block;
        }
        h1,
        h2,
        h3 {
            margin: 0;
            background-color: rgba(0, 0, 0, .5);
        }
    ```
5. 每条规则结束后都必须加上分号
6. 如果属性值为0，则不需要为加单位
7. 去掉uri中引用资源的引号
8. 私有属性在前标准属性在后，向后兼容
9. 避免使用hack
10. 属性合并

## JavaScript

1. 使用对象或数组字面量代替new关键字
2. 禁止使用关键字或保留字命名变量或对象属性
3. 书写格式
    - 赋值或运算符前后需要空格；
    - 大括号前或逗号后需要空格；
    - 对象属性需换行；
    - 前置大括号紧跟小括号之后；
    - 省略对象属性名的引号，除了拼接属性名

    ```javascript
        //不建议
        const atom={
          value:1,
          addValue:function(value){
            return atom.value+value;
          },
        };

        //建议
        const atom = {
          value: 1,
          addValue: function(value) {
            return atom.value + value;
          },
        };
    ```
4. 对字符串使用单引号
5. 避免使用eval
6. 减少全局变量
7. 单个变量定义
8. 数组长度缓存
9. 脚本文件放置body结束标签之前


## 图像约定

1. 所有图片必须经过一定的压缩和优化才能发布
2. 选择正确的图片格式
3. 选择正确的图片引用方式
4. 合理使用sprites技术
5. 使用字体图标功能
