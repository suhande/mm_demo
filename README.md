
# Markdown示例-suhan
[TOC]

## Markdown简介
------
**Markdown**是一种轻量级标记语言，创始人为 John Gruber。它允许人们「使用易读易写的纯文本格式编写文档，然后转换成有效的 XHTML（或者 HTML）文档」：
### 1. Markdown优点
- **学习成本低** ——身为一个轻量级的标记语言，Markdown拥有较少的标记符号，经常用到的就更少了，而且非常简单。
- **任何文本编辑器都可以打开**  ——Markdown文档实际上就是纯文本（plain text）格式，只要是个文本编辑器都可以打开，只不过支持Markdown语法的编辑器会将其渲染成相应格式，由于其语法足够简单，即使用不支持Markdown的编辑器打开，你也能看懂。
- **学习成本低** 格式转换方便 ——不少Markdown编辑器支持将文档转为pdf、docx、html等，你也可以使用具有瑞士军刀之称的Pandoc轻松将Markdown文档转为其他格式
- **你可以更多地关注内容** ——用富文本编辑器编辑文档的话，你的精力往往过多分散到排版上，有的人甚至逐句调整格式，学会Markdown的话，你的注意力又会重新转移到内容上来
- **像记事本一样的速度** ——在Windows上办公时，我常常想，如果用记事本码字就好了，因为其打开速度实在是太快了。但记事本里的文字是没有格式的，体验很差，Markdown格式文档完美继承其速度，又添加了优美的格式。
- **利用Github做版本控制** ——Github不仅仅可以用来托管代码，还可以用来托管文章，而且Github文档默认是Markdown格式的。另外，你还可以利用GitHub与Gitbook写电子书。
### **2. 都是哪些人用markdown？**
- 程序员-写文档
- 学生-记笔记，写论文
- 作家-写文章，写小说
- 博客博主-写博文

Markdown 和 word 各有各的优势，你不能要求一个政府文员、普通的受众去学习使用markdown，markdown相比于word，其默认格式与样式的丰富性远远不如后者，对于复杂的、图文混排、酷炫效果排版等还是让word来做。
### **3. 众多支持Markdown的写作平台**
> *  [Github](https://github.com/suhande/mm_demo)：全球最大开源代码托管平台
> * [有道云笔记][1]
> * [知乎][2]
> * [简书][3]
> * [所有电子邮箱][4]


> * CSDN：程序员博客平台
> *  Wordpress博客



------


## Markdown基本标签

**Markdown**的强大功能：图片和链接嵌入、标题系统及目录生成、多平台支持、微信公众号图文消息一键转换、基本语法与编辑工具、视频及地图嵌入等。将你从繁杂的文字图片排版工作中解放出来，专注内容质量本身。


### 1. 标题
使用#，可表示1-6级标题。
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
### 2. 字体
> *斜体文本*
> _斜体文本_
> **粗体文本**
> __粗体文本__
> ***粗斜体文本***
> ___粗斜体文本___

### 3. 插入图片及链接
![cmd-markdown-logo](https://www.zybuluo.com/static/img/logo.png)


### 4. 制作一份列表([详细教程][2])

- [ ] 支持以 PDF 格式导出文稿
- [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
- [x] 新增 Todo 列表功能
- [x] 修复 LaTex 公式渲染问题
- [x] 新增 LaTex 公式编号功能

### 5. 书写一个LaTex公式[^LaTeX]

$$E=mc^2$$
可以创建行内公式，例如 $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$。或者块级公式：

$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

### 6. 高亮一段代码[^code]

```python
@requires_authorization
class SomeClass:
    pass

if __name__ == '__main__':
    # A comment
    print 'hello world'
```

### 7. 高效绘制 [流程图](https://www.zybuluo.com/mdeditor?url=https://www.zybuluo.com/static/editor/md-help.markdown#7-流程图)

```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```

### 8. 高效绘制 [序列图](https://www.zybuluo.com/mdeditor?url=https://www.zybuluo.com/static/editor/md-help.markdown#8-序列图)

```seq
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

### 9. 高效绘制 [甘特图](https://www.zybuluo.com/mdeditor?url=https://www.zybuluo.com/static/editor/md-help.markdown#9-甘特图)

```gantt
    title 项目开发流程
    section 项目确定
        需求分析       :a1, 2016-06-22, 3d
        可行性报告     :after a1, 5d
        概念验证       : 5d
    section 项目实施
        概要设计      :2016-07-05  , 5d
        详细设计      :2016-07-08, 10d
        编码          :2016-07-15, 10d
        测试          :2016-07-22, 5d
    section 发布验收
        发布: 2d
        验收: 3d
```

### 10. 绘制表格

| 项目        | 价格   |  数量  |
| --------   | -----:  | :----:  |
| 计算机     | \$1600 |   5     |
| 手机        |   \$12   |   12   |
| 管线        |    \$1    |  234  |

### 11. 更详细语法说明

想要查看更详细的语法说明，可以参考我们准备的 [菜鸟网站 Markdown 教程][5]， 



作者 [@suhan][3]     
2016 年 07月 07日    

**以下是注脚：**
[^LaTeX]: 支持 **LaTeX** 编辑显示支持，例如：$\sum_{i=1}^n a_i=0$， 访问 [MathJax][4] 参考更多使用方法。

[^code]: 代码高亮功能支持包括 Java, Python, JavaScript 在内的，**四十一**种主流编程语言。

  [1]: http://maxiang.info/client_zh
  [2]: https://www.runoob.com/markdown/md-lists.html
  [3]: http://adrai.github.io/flowchart.js/
  [4]: http://bramp.github.io/js-sequence-diagrams/
  [5]: https://www.runoob.com/markdown/md-tutorial.html

