## WinEdt10.3 个性化设置

![截图](https://github.com/maboloshi/WinEdt-10-User-Settings/raw/shots/shots/WinEdt_10_%E6%B1%89%E5%8C%96%E8%8F%9C%E5%8D%95.gif)

### 功能简介
#### 相对于默认设置:

1. 添加对`LaTeXMK`的支持<sup>[1](#latexmk)</sup>, 默认引擎为`XelaTeX`
1. 添加 [Floats](http://www.winedt.org/config/tree/Floats.html) 插件
1. 汉化部分常用菜单, 保留不太好翻译的菜单
1. 使用内部宏插入图片功能
1. 内置pdf浏览器 [sumatrapdf x64](https://www.sumatrapdfreader.org/)
1. 添加[在线制表工具](https://www.tablesgenerator.com/latex_tables)
1. 添加编译生产术语表功能
1. 自定义主菜单, 工具栏, 字体设置等
1. 修改添加一些 tex 模板示例

> 参考:

1. <a name="latexmk"></a>[Winedt 一键编译 LaTeX 文档](https://www.twblogs.net/a/5b8f04362b71771883494ef9)
2. [Using Latexmk](https://mg.readthedocs.io/latexmk.html)

#### 相对于其他个性化版本:

1. 移除 [Xy-pic](http://www.winedt.org/old/Config/GUI/Xy-pic.php) 插件绘制二维交换图
1. 移除 TexFriend 工具
1. 移除 [QuadView](https://zohooo.github.io/quadview/) 工具
1. 移除内置 GSview 工具
1. 移除 [Graphics](http://www.winedt.org/old/Plugins/graphics.php) 插件
1. 移除 [complete](http://www.winedt.org/old/Plugins/complete.php) 插件
1. 移除 CCT相关工具 如 cct*, gbk2uni
1. **尊重版权不添加无限试用设置**
1. 不包含`winedt.dnt`设置文件, 自行重建即可


### 重建`winedt.dnt`设置

菜单栏`Options`-->`Maintenance`-->`Rebuild All...`

### Tex发行版设置
> 此处以 MiKTeX 便携版为例

#### 手动设置

菜单栏`Options`-->`Execution Modes`, 在弹出的对话框中选择`TeX System`选项卡, 点击`TeX Root`附近的放大镜图标, 选择 MiKTeX 根目录(例如: `G:\miktex-portable\texmfs\install`) 然后点击`Apply`

> 注意:
> 根据实际是否勾选`Maintain MiKTeX as Administrator` (即是否以管理员权限运行 MikTeX 控制台)

同理, 可以在`PDF Viewer`和`Ghostscript`设置PDF浏览器和GS浏览器路径

#### 验证设置
接上述, 切换至`Diagnosis`选项卡, 点击底下的`Diagnose the System`, 查看自动检测生成的报告. 相关二进制工具是否找到, 相关缺失的工具是否对你有影响.

### 其他设置
#### 文件类型关联
菜单栏`选项`-->`设置向导`, 在弹出的对话框中选择`Filetype Associations`选项卡, 点击`Modify filetype associations..`, 然后根据需要进行文件类型关联.