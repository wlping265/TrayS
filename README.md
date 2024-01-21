[toc]

# 使用技巧

## 常用快捷键

Typora 中文网：https://www.typora.net/support/

| 功能描述      | 快捷键   |
| :-------------- | -------- |
| 源代码模式 切换 | `Ctrl + /` 或 点击界面左下角 </> |
| 专注模式 切换 | F8 |
| 显示/隐藏侧边栏 | Ctrl + Shift + L |
|  |          |
| 保存 | Ctrl + S |
| 复制/粘贴/剪切/全选 | Ctrl + C/V/X/A |
| 粘贴为 MarkDown | Ctrl + Shift + C |
| 粘贴为纯文本 | Ctrl + Shift + V |
| 撤销/重做         | `Ctrl + Z/Y` |
| 选中当前行 | Ctrl + L |
| 清除样式 | Ctrl +　\ |
| 查找 | Ctrl + F |
| 替换 | Ctrl + H |
| 查找下一个/下一个 | F3 / Shift + F3 |
|  |  |
| 插入表格 | `Ctrl + T` |
| 表格当前行下方增加一行 | `Ctrl + Enter` |
| 表格或代码中内容换行 | `Shift + Enter`   |
| 移动表格当前行或列 | Alt + 上/下/左/右 (也可以 `通过鼠标放到行/列的最左/上边框进行拖动`) |
| 删除表格当前行 | Ctrl + Shift + 退格 |
| 表格左对齐： | 源码模式下在表格标题栏--------前加: 号，如 :-------- <br /> `点击表格顶部对齐按钮` |
| 表格右对齐： | 源码模式下在表格标题栏--------后加: 号，如 --------: <br /> `点击表格顶部对齐按钮` |
| 表格居中对齐： | 源码模式下在表格标题栏--------两端加: 号，如 :--------: <br /> `点击表格顶部对齐按钮` |

## 常用样式及快捷键

| 样式           | 语法格式                   | 快捷键                  |
| -------------- | --------------------------------- | ----------------------- |
| 目录（效果见文首） | `[toc]空格` | Table of Contents(TOC) |
| 标题 最多 6 级（效果见文末） | `## 文本`（#号个数对应标题级数） | Ctrl + (1,2,3,4,5,6,0) <br /> 数字对应标题级别，0 表示正文段落 |
| 降低标题级别/提升标题级别 |  | Ctrl + - / Ctrl + = |
| 有序列表（效果见文末） | `数字. 文本` | Ctrl + Shift + [ |
| 无序列表（效果见文末） | `- 文本` | Ctrl + Shift + ] |
| 任务列表（效果见文末） | `- [ ] 文本 /- [X] 文本` | Ctrl + Shift + X |
| 引用文本（效果见文末） | `> 文本`                         | Ctrl + Shift + Q        |
| 分割线（效果见文末） | `---` 或 `***`                    |                         |
| *斜体*         | `*文本*`                        | ctrl + I               |
| **加粗** | `**文本**` 或者 `__文本__` | ctrl + B               |
| <ins>下划线</ins> <u>文本</u> | `<u>文本</u>` 或`<ins>text</ins>` 后者是建议用法 |                                                              |
| ~~删除文本~~ | `~~文本~~`                      | Alt + shift + 5         |
| [超链接](http://www.baidu.com) | `[文本](链接地址)`       |Ctrl +　K <br /> 链接地址换成 `#文档内的标题` <br /> 或者 `#文档内html标签id或name属性值`(建议用 a 和 span)<br /> 可以实现文档内跳转|
| URLs 例：<www.baidu.com> | `<www.baidu.com>`                  | <链接> 支持链接标准的 URLs |
| `行内代码` | [\`文本\`]() |Ctrl + Shift + \`|
| 代码块（效果见文末） | \`\`\`语言类型<br />代码块<br />\`\`\` |Ctrl + Shift + K(快捷键冲突)|
| 表情 :happy: :cactus:`（与GFM有差异）` | `:happy: :cactus:` | 英文模式下，输入冒号再输入第一个字母开始会提示选项 <br /> 微软输入法可以用 `Ctrl + Shift + B` 弹出表情窗口 |



## 部分 HTML 样式

**在 Markdown 诞生之初，它就是为了被浏览器阅读而设计的**, Typora 利用解析器先将我们写的 Markdown 文档解析成为 HTML 文档, 通过 js 和 css 赋予多种样式, 所以是支持输入 html 标签和代码块的，例如下面是一部分基础 html 样式语法

| 样式           | 语法格式                   | 描述                |
| -------------- | --------------------------------- | ----------------------- |
| <kbd> 圆角矩形框 </kbd> | `<kbd>文本</kbd>` ||
| <font color=blue> 字体颜色 </font> | `<font color=blue>文本</font>` | 可以是颜色 16 进制格式 #008000 |
| <font size=4> 字体大小 </font> | `<font size=4>文本</font>`    |                         |
| <font face="华文彩云"> 文字字体 </font> | `<font face="华文彩云">文本</font>` |             |
| 下标 <sub> A </sub>         | `<sub>文本</sub>`                 |                         |
| 上标 <sup> A </sup>         | `<sup>文本</sup>`                 |                         |
| 文本居中（样式见下文） | `<center>文本</center>` ||
| <span style="background:grey;"> 文字背景色 </span> | `<span style="background:grey;">文本</span>` ||

## 扩展语法

要使用扩展语法 `需要在设置中MarkDown扩展选项打开相关选项`，包括 公式、上标、下标、文字高亮

| 样式                                   | 语法格式                                   |
| -------------------------------------- | ------------------------------------------ |
| ==高亮== `（非GFM标准）`                    | `==文字==`                                 |
| 上标(公式样式不适用) y^2^= 4 `（非GFM标准）` | `^文字^ 例：y^2^=4`                        |
| 下标(公式样式不适用) H~2~O `（非GFM标准）`  | `~文字~ 例：H~2~O`                         |
| 内联公式 $\lim_{x\to\infty}\exp(-x)=0$ | `$公式$ 例：$\lim_{x\to\infty}\exp(-x)=0$` |
| 公式块(居中, 见下文公式举例)`（非GFM标准）` | `$$` <br /> 公式 <br /> `$$`                   |

### 各种公式语法举例(支持 LaTeX)

==`$\frac{7x+5}{\sqrt{1+y^2}}$`== -> $\frac{7x+5}{\sqrt{1+y^2}}$

==`$z=z_l$`== -> $z = z_l$

==`$\sqrt{2}$`== -> $\sqrt{2}$

==`$\sqrt[n]{3}$`== -> $\sqrt[n]{3}$

==`$\cdots$`== -> $\cdots$

==`$\vec{a}\cdot\vec{b} = 0$`== -> $\vec{a}\cdot\vec{b}=0$

==`$\int^2_3x^2{\rm d}x$`== -> $\int^2_3x^2{\rm d}x$

==`$\lim_{n\rightarrow+\infty}n$`== ->  $\lim_{n\rightarrow+\infty}n$

==`$\frac{1}{i^2}$`== -> $\frac{1}{i^2}$

==`$\prod\frac{1}{i^2}$`== -> $\prod\frac{1}{i^2}$

==`$\frac{d}{dx}e^{ax}=ae^{ax}\quad\sum_{i = 1}^{n}{(X_i-\overline{X})^2}$`== -> 
	$\frac{d}{dx}e^{ax}=ae^{ax}\quad\sum_{i = 1}^{n}{(X_i-\overline{X})^2}$



```tex
\mathbf{V}_1 \times \mathbf{V}_2 =
\begin{vmatrix}
\mathbf{i}& \mathbf{j}& \mathbf{k} \\
\frac{\partial X}{\partial u}& \frac{\partial Y}{\partial u}& 0 \\
\frac{\partial X}{\partial v}& \frac{\partial Y}{\partial v}& 0 \\
\end{vmatrix}
```

根据上方代码块中的公式，输入到公式块效果展示如下：
$$
\mathbf{V}_1 \times \mathbf{V}_2 =
\begin{vmatrix}
\mathbf{i}& \mathbf{j}& \mathbf{k} \\
\frac{\partial X}{\partial u}& \frac{\partial Y}{\partial u}& 0 \\
\frac{\partial X}{\partial v}& \frac{\partial Y}{\partial v}& 0 \\
\end{vmatrix}
$$

## 流程图`（非GFM标准）`

参考：https://baijiahao.baidu.com/s?id=1680509829195209918&wfr=spider&for=pc

在代码块里输入流程的代码，并选择代码语言为 flow，即为流程图效果，

用markdown写流程图还是有些不那么方便直观，不如直接使用流程图绘制工具画好之后截图使用，专业的事交给专业的软件去做

### 流程图语法

流程图大致分为两段，第一段是定义元素，第二段是定义元素之间的走向。

#### 元素定义语法

```
tag=>type: content:>url
```

- tag 就是元素名字，
- type 是这个元素的类型，有 6 中类型，分别为：
  - start # 开始
  - end # 结束
  - operation # 操作
  - subroutine # 子程序
  - condition # 条件
  - inputoutput # 输入或产出
- content 就是在框框中要写的内容，注意 type 后的冒号与文本之间一定要有个空格。
- url 是一个连接，与框框中的文本相绑定

#### 连接元素的语法

用 **->** 来连接两个元素，需要注意的是 condition 类型，因为他有 yes 和 no 两个分支，所以要写成

```
c2(yes)->io->e 
c2(no)->op2->e
```

### 效果示例

==代码 1==

```
st=>start: 开始
ipt=>inputoutput: 输入一个x
op=>operation: 处理加工x+1
cond=>condition: 溢出（是或否？）
sub=>subroutine: 子流程
io=>inputoutput: 输出x
ed=>end: 结束
st->ipt->op->cond
cond(yes)->io->ed
cond(no)->sub->io->ed
```

==效果 1==

```flow
st=>start: 开始
ipt=>inputoutput: 输入一个x
op=>operation: 处理加工x+1
cond=>condition: 溢出（是或否？）
sub=>subroutine: 子流程
io=>inputoutput: 输出x
ed=>end: 结束
st->ipt->op->cond
cond(yes)->io->ed
cond(no)->sub->io->ed
```

==代码 2==

```
flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: get_hotel_ids|past
op2=>operation: get_proxy|current
sub1=>subroutine: get_proxy|current
op3=>operation: save_comment|current
op4=>operation: set_sentiment|current
op5=>operation: set_record|current

cond1=>condition: ids_remain空?
cond2=>condition: proxy_list空?
cond3=>condition: ids_got空?
cond4=>condition: 爬取成功?
cond5=>condition: ids_remain空?

io1=>inputoutput: ids-remain
io2=>inputoutput: proxy_list
io3=>inputoutput: ids-got

st->op1(right)->io1->cond1
cond1(yes)->sub1->io2->cond2
cond2(no)->op3
cond2(yes)->sub1
cond1(no)->op3->cond4
cond4(yes)->io3->cond3
cond4(no)->io1
cond3(no)->op4
cond3(yes, right)->cond5
cond5(yes)->op5
cond5(no)->cond3
op5->e
```

==效果 2==

```flow
flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: get_hotel_ids|past
op2=>operation: get_proxy|current
sub1=>subroutine: get_proxy|current
op3=>operation: save_comment|current
op4=>operation: set_sentiment|current
op5=>operation: set_record|current

cond1=>condition: ids_remain空?
cond2=>condition: proxy_list空?
cond3=>condition: ids_got空?
cond4=>condition: 爬取成功?
cond5=>condition: ids_remain空?

io1=>inputoutput: ids-remain
io2=>inputoutput: proxy_list
io3=>inputoutput: ids-got

st->op1(right)->io1->cond1
cond1(yes)->sub1->io2->cond2
cond2(no)->op3
cond2(yes)->sub1
cond1(no)->op3->cond4
cond4(yes)->io3->cond3
cond4(no)->io1
cond3(no)->op4
cond3(yes, right)->cond5
cond5(yes)->op5
cond5(no)->cond3
op5->e
```





## 部分样式展示

文中常用样式列表中无法直观看到样式的展示在下边

---

`> 引用文本` 第一层需要顶格开始

> 文本
>
> > 嵌套引用
> >
> > > 再套个娃
> >
> >
>
>



---

`<center>文本居中</center>`


<center> 文本居中 </center>

---

代码块

```java
Hello Word!
```

---

`列表两个空格代表一层缩进`，可以手打，也可以通过选中列表的某一条或者多条，按 Tab 增加缩进，按 Shift + Tab 减少缩进

1. 有序列表 `数字. 文字`
2. 有序列表
3. 有序列表

- 无序列表(无缩进) `- 文字`
  - 无序列表(一格缩进)
    - 无序列表(两格缩进)
    - 无序列表



- [ ] 任务列表 `- [ ] 文字`
- [x] 任务列表 `- [X] 文字`
- [ ] 任务列表

---
**标题**

# # 一级标题

## ## 二级级标题

### ### 三级级标题

#### #### 四级级标题

##### ##### 五级级标题

###### ###### 六级级标题

另一种写法，采用 Html 的标题标签 `<h数字>数字代表标题级别</h数字>` , 效果如下：

<h1> h1 标题 </h1>
<h2> h2 标题 </h2>
<h3> h3 标题 </h3>
<h4> h4 标题 </h4>
<h5> h5 标题 </h5>
---

`[^脚注名字] [^脚注名字]:脚注内容` 

注释示例 [^1]

[^1]: 注释可以鼠标悬停显示

---

