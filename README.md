### 更新进度

#### 0.34版本

- 修复切换标签页时导致没有正常出现列表转表格等功能的bug
- 修复面包屑右侧出现滚动条的bug

#### 0.33版本

- 修复反链面板显示更多时文字拥挤错乱bug
- 修复钉住标签页时红点显示不圆的问题
- 修改PDF双链样式，将边框修改为文字下划线
- 一级标题和分割线打印时自动添加分页
- 导出为PDF时去掉标题前面的“H1”等标识

#### 0.32版本

- 修复思源笔记默认主题更新导致的兼容性问题
- 取消显示标签页上的图标
- 为钉住的标签页右上角添加红点标识
- 优化了一些细节

#### 0.31版本

- 增加一个文档自定义属性 f=heng ,将其设置为横版A4纸页面
- 增加一个文档自定义属性 f=full，可以将页面设置为全屏
  - #注意 设置了以上两个自定义属性，标题和题头图的位置不会发生改变，因为自定义属性仅对正文区域有效

- 在主题文件夹增加一个 custom.css 文件，**将其中的代码取消注释，可永久实现全屏**，而不是只有 A4 纸大小
  - 目前存在的问题：标题和正文之间可能存在较大空隙
    - 如果想要解决这个问题，每次更新都需要删除 theme.css 文件中的 A4.css 一行，然后再保存
    - 如果之后解决了这个问题，不需要每次更新都重新设置，会在集市说明文档中进行强调

- 为导出属性增加一个属性值 f=print（打印）；导出样式 f=print 或者 f=daochu（导出） 都行
  - 导出 PDF 样式和自定义属性还是有很大差异，仅供参考
  - 目前导出 PDF 不管有没有设置自定义属性，默认都是标题为黑体，段落为宋体，英文为 Times 字体
    - 想取消掉此设置，需要将 theme.css 代码里边的 print.css 一行删除掉，再保存即可

#### 0.3版本

- 修改代码块样式
- 增加 Roy 的 js 脚本

#### 之前版本

- 增加了列表转思维导图的功能（来自于 Roy 的源代码和萌新的修改）
- 给表格增加了横向边框
- 优化待办事项样式（折叠也有不同样式）
- 修复有序列表折叠后不显示数字的 bug
- 通过文档的自定义属性 f=full,可以将页面调整至全宽
- 优化了一些细节

### 感谢列表

* 本主题从 zhang-light 主题修改而来
* 缝合了 Roundark 主题的标签页样式和 BearLight 主题的一些设计
* 感谢 Rc 和 weihan-Chen 在标签页功能上给予的帮助
* 搜索界面采用左右分栏，使用了链接社区 abbj 的代码
* 感谢 Roy 开发的列表转思维导图的功能和萌新的修改；感谢九炎大佬提供的js脚本，可以省略输入自定义属性这个步骤

### 使用说明

* 本主题致力于无限接近于所见即所得，方便大家导出为PDF
  * 现阶段还做不到完全一致

* 本主题强制限制页面宽度为 21cm, 为 A4 纸的宽度
* 页边距可以通过修改 CSS 进行设置
* 导出PDF时，预览样式和导出样式存在一定误差，不是 100% 相同
* 各种自定义属性和设置和 zhang-light 主题保持一致
* 本主题将各种类型的代码块都进行了拆分，方便大家进行修改
* 有一些 zhang-light 主题的功能并没有加到本主题中
  * 比如链接前面的icon图标
  * 比如“/”分栏


### Style 文件夹代码分类

| 分类                      | 解释           | 分类                         |
| --------------------------- | ---------------- | ------------------------------ |
| color-font                | 颜色和字体     |                              |
| appearance                | 界面外观       | 包含文档树，标签页，面包屑等 |
| inline-span               | 行内元素       | 包含标签，行内代码，高亮等   |
| block-div                 | 块级元素       | 包含表格，引用，代码块等     |
| custom-function-for-file  | 文档自定义属性 |                              |
| csutom-function-for-block | 块的自定义属性 |                              |
| others                    | 其他样式       |                              |

### Chrome-A4 主题专属属性

| 名称              | 属性                  | 备注 |
| ----------------- | --------------------- | ---- |
| A4纸横排          | f=heng                |      |
| 页面全宽          | f=ful                 |      |
| 导出样式/打印样式 | f=daochu 或者 f=print |      |



### 列表转表格/思维导图用法

- 点击列表左上角图标，在弹出窗口中可以选择显示为导图，显示为表格，显示为默认
  - 属性值为 f=dt(导图)，f=bg(表格)

![列表转导图.gif](https://tva1.sinaimg.cn/large/0082QUidly1h236c9w14jg312j0rj7cc.gif)

### 图片展示

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zd9vihsj31hc0smdmu.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zhob47xj31hc0smnbd.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zjouv7sj31hc0sm46x.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zk6bjogj31hc0smn5q.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zm61xdnj31hc0smx4o.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zo3wn3pj31hc0smtij.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zp7rho7j31hc0sm7bz.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zpucx5fj31hc0sm4gg.jpg)

![image.png](https://tva1.sinaimg.cn/large/0082QUidly1h14zs6jrdmj31hc0smdr6.jpg)
