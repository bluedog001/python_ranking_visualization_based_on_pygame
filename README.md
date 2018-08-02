# 动态排名数据可视化
一个基于pygame的数据可视化工具，可以直观并较为美观的展示出历史数据排名的情况

请注意：此项目是一个js项目的再现，原项目地址：https://github.com/Jannchie/Historical-ranking-data-visualization-based-on-d3.js
----
# 使用方法
根目录下存在已经编译好的exe文件(main.exe)，双击打开，输入csv文件路径或者直接将csv文件拖入，按下回车即会开始输出图像。

如果您的电脑上有python解释器，并有安装pygame模块，可以打开根目录下的脚本文件(main.py)，具体使用方法与exe相同。

# 数据格式
本项目目前只可以读取csv文件

数据格式与原项目基本相同：

name|type|value|date

名称1|类型1|值1|日期1

名称2|类型2|值2|日期2


其中名称会显示在柱状图左侧以及柱状图末端，类型会在该条目处于榜首时显示。

值通常认为是一个正整数，也可以是一个浮点数。

本项目会在读取时对date进行基于字符串的正序排列，所以数据源可以是乱序的，但是请注意数据源提供的日期是否符合字符串排序规则。建议使用YYYY-MM-DD的格式

# 个性化
本项目可以进行有限的个性化修改。

使用任意文本编辑器打开源码(main.py)，在文件顶部可以看到使用"#"分隔的常量区，可以依照注释对需要的部分进行微调。

# 细节及其他
本项目默认帧率为60fps，代码内所有表示时长的均使用单位frame(s)。如30代表0.5秒，45代表0.75秒。

因为使用游戏引擎渲染，并不能完全保证展示过程中不会出现卡顿。

图片输出功能尚在开发中。

----
# 更新日志
## 2018-8-2
- 整体框架
- 使用HSV颜色选择器，使得随机颜色选择更加平滑和谐
