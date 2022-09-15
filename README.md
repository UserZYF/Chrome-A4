### 使用说明

- 主题主打简洁，整体色调偏白，模仿 Chrome 浏览器的标签页设置（后期会将宽度限制为 A4 纸大小）

- 自定义属性等和 Zhang-light 主题一致

- 学习 Notion 主题相关代码，隐藏了顶栏

### 反馈渠道

> - GitHub 主页或者 QQ：3466181911

### 更新进度

#### 0.35版本

* 取消 A4 宽度的限制，Copy notion 主题的顶栏设计，隐藏顶栏
* 将侧栏和文档树位置整体下移（设置 padding）
* 重新对标签页相关代码进行设计
* 参考 Chrome 浏览器的颜色设计标签页
* 增加标签页高度， 减少面包屑高度
* 缩小面包屑文字和符号大小
* 面包屑 focus 加入背景颜色
* 取消标题前面的“H1”等符号
* 去除 list 底部边距的代码
* 修复不显示通知的 bug
* 列表块标和文字位置不对应的 bug
* 左侧和右侧 dock 栏设置成白色，这样收缩时更加融为一体
* 隐藏文档树滚动条，鼠标悬浮时显示
* 修改 on/off 按钮样式
* 确定主题色是蓝色还是红色
  * 如果是模仿 Chrome 主题的话，还是蓝色更加合适一点
  * 主题色：`#4285f4`
    * 可以用在块引用文字颜色上面
  * 蓝紫色：`#6d7ec8` 来自于 wps
    * 可以用在固定标签页中，替换原本的粉色
* 增加列表折叠颜色深度
* 增加默认英文字体
  * inter 字体官网
    * https://rsms.me/inter
    * 免费可商用
  * 在 README 中进行声明
* 修改新建文档按钮悬浮时的颜色
  * 正在等待颜色发生变化
  * 未发生变化，鼠标 hover 时颜色不发生变化
* 修改块引用样式（降低块引用的高度）
* 修改超链接样式
* 将底部状态栏设置为白色
* 给标题增加明显的级别
  * 可以加上三个点
* 取消设置界面打开主题文件夹下方的横线
* 将阴影设置为默认的数值大小
* 修改高亮样式颜色
* 修改代码块样式
  * 要求简约一点
* 去除PDF等超链接前面的汉字描述
* 修改PDF双链样式

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


### Style 文件夹代码分类

| 分类                      | 解释           | 分类                         |
| ------------------------- | -------------- | ---------------------------- |
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
