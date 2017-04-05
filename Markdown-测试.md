---
title: Hexo-theme-apollo 主题的 Markdown 测试或者说码字教程！？
date: 2017-04-05 20:10:01
tags: Markdown  Blog写作
desc: This is Meta Description test.
---
 Markdown是非常棒以及流行的写作语法，平文本，「易读易写」，一般只需几分钟就能学会Markdown的基本用法。本文意在测试apollo模板中的各种Markdown显示效果。本人日常写作环境为MarkEditor，故以MarkEditor官方帮助文档为原本，以原作者GitHub中的参考文档为参考资料，做显示测试。Blog中只能呈现最终效果，原文详见我的Github文档。
Markdown写作的意义就不想谈了前人总结的够好了<http://www.yangzhiping.com/tech/writing-space.html>

<!--more-->

## 加粗 斜体 删除
**用两个星号标记起来，表示加粗**，*一个星号，表示斜体*，~~这样子表示删除~~，这些就是最基本的语法了。

## 关于标题
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
分别对应HTML中的`<h1>一级标题</h1>`，以此类推。


> 实际上，Hexo-theme-apollo 只支持两种标题：h1~h3 大标题，h4~h6 小标题，也就是说，# 和 ### 的样式是一样的。之所以这么处理，是因为就个人感觉而言，我们不应该为文章设置过多的层级消耗读者的阅读精力。这相当于强制使用 Hexo-theme-apollo 的用户在写文章时注意文章结构，最多只能使用两层结构。另一个潜在的原因是因为我还没有发现好的样式来处理不同层级的标题，单纯以大小和颜色很容易让页面变得混乱和冗杂。（引自作者说明文档）

<div class="tip">
  测试效果，一级文档前并没有#，所以实际上还是有三级标题可以使用，配合后文介绍的列表，应该已经可以相对丰富的呈现文章的层次了。
</div>

## 列表

**无序列表:** 使用 -
-   Red
-   Green
-   Blue

**无序列表:** 使用 *
* A
* B
* C

**有序列表则使用数字接着一个英文句点：**
1.  Bird
2.  McHale
3.  Parish

**也可以混合在一起使用:**

-   Bird
    - blue bird
-   McHale
    1.  a man
    2.  HoustonRockets
-   Parish
<div class="tip">
我也是第一次知道无序列表的 - 和 * 两种 标记。模版中正常显示
</div>

## 内容引用
用`>`放在段首，之后是空格，输入文字:

> 你
> 一会看我
> 一会看云

>  我觉得
>  你看我时很远
>  你看云时很近


<div class="tip">
上文引用作者的话使用过。
</div>

## 插入链接
**插入链接:**
这是一个 [链接 apollo作者的GitHub的参考](https://github.com/pinggod/hexo-theme-apollo/blob/master/doc/doc-zh.md)

**快速链接:**
只需要在网址头尾用尖括号包裹即可，比如<https://github.com/aptx4869yuyang2017> 
我的GitHub，欢迎follow👏。


## 分割线
**`-`加上空格组成，三个以上:**
- - - - - -
本Theme不支持

# 以下是Hexo-theme-apollo的特别支持的部分  直接全文引用了 
## Meta Description
如果你想设置页面的 meta description 信息，请在每篇 markdown 文件的头部添加 desc 字段信息——更实用的方式是在 scaffolds 文件夹中，将 desc 配置到常用模板中去，示例如下：
```md
title: Lorem ipsum dolor
date: 2015-12-31 14:49:13
desc: Lorem ipsum dolor sit amet, consectetur.
---

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!
```

生成结果:

```html
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">
```

如果没有配置该信息，Hexo-theme-apollo 会使用 `page.title` 和 `page.author` 来配置该标签。

## 文章摘要

如果你想创建文章摘要用于向读者展示文章的核心内容，那么需要在文章摘要之后其他内容之前添加 HTML 注释标签 `<!--more-->`，使用方法如下图所示：

![https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png](https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png)

<div class="tip">
第一段我就当摘要用了。
</div>

## 评论插件

Hexo-theme-apollo 支持两种评论插件：Disqus 和 Duoshuo. 请在 `theme/_config.yml` 文件中做如下配置:

```yaml
disqus: seansun
```

<div class="tip">
开启没成功，以后再研究吧。
</div>

## 警告块

使用警告块需要 `div` 标签和 `tip` 类名：

```html
<div class="tip">
    预处理器很强大，但它只是编写 CSS 的辅助工具。出于对扩展和维护等方面的考虑，在大型项目中有必要使用预处理器构建 CSS；但是对于小型项目，原生的 CSS 可能是一种更好的选择。不要肆意使用预处理器！
</div>
```
<div class="tip">
文章中我的分析基本都用警告块了。
</div>

![danger](https://cloud.githubusercontent.com/assets/9530963/11359678/489a510c-92b9-11e5-9256-341cef6999b6.png)

## 参考资料
作者的中文参考文档 <https://github.com/pinggod/hexo-theme-apollo/blob/master/doc/doc-zh.md>
本文是本主题下的显示效果  ，一般效果和没有渲染的版本请看 <https://github.com/aptx4869yuyang2017/apollo-Test/blob/master/Markdown-%E6%B5%8B%E8%AF%95.md>


