---
marp: true
theme: NUDTSce
paginate: true
math: katex
---

<!--
_paginate: false
-->
![bg vertical w:1300px](./images/封面1.png)
<br/>
<br/>
<br/>

# 汇报题目 h1样式
## 副标题 h2样式
**学员 2026-04-13**
**导师1 导师2**
**国防科技大学 前沿交叉学科学院**


---
<style scoped>
    section {
  text-align: center;
    }
    h1 {
        color: rgb(1, 87, 68);
        margin-bottom: 30px;
    }
    h6 {
        text-align: center;
    }

</style>
<!--
_paginate: false 
-->

![bg left:55% ](./images/cover1.png)
# 目 录

###### 1 Slide 概述
###### 2 文字展示
###### 3 代码展示
###### 4 公式展示
###### 5 表格展示
###### 6 图片展示
###### 7 其它展示
###### 8 参考文献&引用展示


---
<!-- _header: 1 Slide概述 -->

本PPT借助插件Vscode插件Marp书写而成，由markdown文档编辑，方便公式和代码的展示与排版。

**环境：**
- 系统：Win10/11
- 软件：VsCode/Cursor 插件：Marp
- theme：自定义主题 NUDTSce ，基于中国科学院大学Marp-Theme-UCAS主题修改
  

**特征：**
- 背景选用科大风景，每页上方标题栏基于Marp header格式进行修改而成。
- 首尾页和目录页图片基于背景得到，首尾页可根据文字内容在本页修改标题样式，目录页可根据文字内容对图片进行大小位置调整

---
<!-- _header: 1 Slide概述（续） -->

**快速上手流程：**
1. 复制本模板并修改封面页标题、作者、日期信息。
2. 按章节新增 `---` 分页，使用 `<!-- _header: 标题 -->` 配置页眉。
3. 在正文中按需插入代码、公式、表格和图片，并预览检查换页位置。
4. 使用 `Marp: Export slide deck...` 导出 PDF / PPTX 版本用于答辩或汇报。

**写作建议：**
- 一页只表达一个核心观点，正文保持 4~8 行为宜。
- 图表页尽量“图大字少”，结论放在页眉下方第一行。
- 目录和章节过渡页可以沿用本模板，保持整套视觉统一。

---
<!-- _header: 2 文字展示 -->
**h1 h2 只在首页应用 h6 只在目录页应用**
### h3 标题文字
#### h4 标题文字
**加粗文字**
普通文字
*斜体文字*
~~删除线~~

`==高亮文字==`（部分渲染器支持）

> 引用块：用于结论、定义或政策原文摘录

- 无序列表项 A
- 无序列表项 B
1. 有序列表项 1
2. 有序列表项 2

---
<!-- _header: 2 文字展示（续） -->

**文字排版建议：**
- 中英文之间保留空格，数字与单位间建议加空格（如 `10 ms`）。
- 关键词统一使用加粗，不建议同页混用过多颜色。


---
<!--_header: 3 代码展示 -->

### 行内代码展示
行内代码展示 `this is a code`

### 代码块展示
**python code**

``` python
# python code 
import torch

def Net()

```

---
<!--_header: 3 代码展示（续） -->

**代码页建议：**
- 代码块使用语言标识（如 `python`/`cpp`/`bash`）获得高亮。
- 单页代码行数建议不超过 20 行，关键行可用注释标注。
- 终端命令建议单独成行，便于观众快速识别。

```bash
# 示例：导出 PDF
marp Scenery.md --pdf
```
---
<!--_header: 4 代码展示 -->

**C++ code**
``` C++
//c++ code 
#include<iostream.h>
#include<string.h>
using namespace std;

int main(
    cout<<"hello world!";
    return 0;
)

```

**跨语言展示建议：**
- 对比类内容可采用“同一页双代码块”展示输入/输出或新旧实现。
- 若代码较长，拆分为“核心逻辑页 + 结果页”更利于讲解节奏。
---
<!--_header: 5 公式展示 -->

行内公式 $123$

行间公式：

$$
D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases} 
$$

注意：行间公式的编号适配不是很好，加编号会排版错乱

---
<!--_header: 5 公式展示（续） -->

常见公式示例：

- 均值：$\bar{x} = \frac{1}{n}\sum_{i=1}^{n}x_i$
- 方差：$\sigma^2=\frac{1}{n}\sum_{i=1}^{n}(x_i-\bar{x})^2$

矩阵示例：

$$
A=\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

**公式页建议：**
- 单页主公式不超过 2 个，推导过程可拆分多页。
- 变量含义尽量在公式下方用一句话说明。
- 公式查询链接：
  - KaTeX Supported Functions: https://katex.org/docs/supported.html
  - LaTeX Math Cheat Sheet（Overleaf）: https://www.overleaf.com/learn/latex/Mathematical_expressions
  - 手写符号反查（Detexify）: https://detexify.kirelabs.org/classify.html

---
<!--_header: 6 表格展示 -->

复杂表格示例（课程成绩与过程记录）：

| 学号 | 姓名 | 方向 | 平时(30%) | 期中(20%) | 期末(50%) | 总评 | 备注 |
| --- | --- | --- | ---: | ---: | ---: | ---: | --- |
| 2026001 | 张三 | 智能系统 | 92 | 88 | 90 | 90.0 | 班级负责人 |
| 2026002 | 李四 | 空天信息 | 85 | 90 | 93 | 89.5 | 含加分项 +2 |
| 2026003 | 王五 | 交叉学科 | 78 | 82 | 86 | 82.2 | 补交 1 次作业 |
| 2026004 | 赵六 | 计算平台 | 95 | 91 | 94 | 93.7 | 免修实验 1 项 |

说明：
- 可通过“分数列右对齐 + 备注列文本说明”同时呈现定量和定性信息。
- 超宽表格建议拆成“基础信息表 + 指标明细表”两页展示。

---
<!--_header: 6 表格展示（续） -->

对齐方式示例：

| 左对齐 | 居中对齐 | 右对齐 |
| :--- | :---: | ---: |
| 文本A | 文本B | 123 |
| 文本C | 文本D | 456 |

**表格页建议：**
- 表头尽量短，复杂说明放在表格下方。
- 数据较多时建议改为图表或拆分成两页。

---
<!--_header: 7 图片展示 -->
<br/>

![img w:300px](images/cover1.png) ![img w:300px](images/cover2.png) ![img w:300px](images/cover3.png) 

---
<!--_header: 7 其它展示 -->
一些表情

:+1: :-1: :smile: :heart: :cry: :sob: :a: :b: :angry: :grin: :tongue: :ru: :us: :cn:

其他常用语法：

- 脚注：`这是内容[^1]`，文末补 `[^1]: 说明文字`
- 注释：`<!-- 仅源码可见，不会在幻灯片中展示 -->`
- 单页指令：`<!-- _class: lead -->`、`<!-- _paginate: false -->`
- 分栏：配合背景定位或 CSS 实现左右布局

---
<!--_header: 8 参考文献&引用展示 -->
<style scoped>   
    h3 {
        text-align:center;
        margin-bottom: 50px;
    }
</style>
### 一些参考& 进一步阅读

> Marp 官方文档 [link](https://marpit.marp.app/markdown)
> 分栏显示  [link](https://github.com/marp-team/marp/discussions/192)
> Marp VSCode教程 [link](https://github.com/marp-team/marp-vscode)
> CAI Marp详细教程博客 [link](https://caizhiyuan.gitee.io/categories/skills/20200730-marp.html#%E5%8A%9F%E8%83%BD)
> theme gaia 源代码 [link](https://github.com/marp-team/marp-core/blob/main/themes/gaia.scss)
> theme uncover 源代码 [link](https://github.com/marp-team/marp-core/blob/main/themes/uncover.scss)

---
<style scoped>
    section {
  text-align: center;
    }
    h1{
        text-align:center;
    }

</style>

<!--
_paginate: false 
-->

![bg vertical w:1300px](images/致谢1.png)
<br/>
<br/>

# 请各位老师批评指正

<br/>

**学员 2026-04-13**
**导师1 导师2**
**前沿交叉学科学院 第一学科交叉中心**

