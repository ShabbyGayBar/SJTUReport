# SJTUReport 示例模板

[![SJTUTeX](https://img.shields.io/github/v/release/sjtug/SJTUTeX?label=SJTUTeX)](https://github.com/sjtug/SJTUTeX) 
[![Join Discussions](https://img.shields.io/github/discussions/ShabbyGayBar/SJTUReport)](https://github.com/ShabbyGayBar/SJTUReport/discussions)

## 欢迎使用上海交通大学课程报告模板

本示例模板是应用上海交通大学学位论文（非官方）LaTeX 文档类 SJTUReport 的一个完整实现。演示了排版中常用的例子，包括公式、表格、算法、参考文献等。配置文件和演示内容等参考了 [@sjtug](https://github.com/sjtug) 的 [SJTUThesis](https://github.com/sjtug/SJTUThesis) 模板。
用户可以参考或者直接基于此示例文档撰写课程报告。

SJTUReport 支持 XeTeX 与 LuaTeX 引擎，字符编码仅支持 UTF-8。

## 获取模板

### 下载模版

普通用户可以直接 `clone` 或者下载 master.zip。

```bash
git clone https://github.com/ShabbyGayBar/SJTUReport.git
```

## 模板使用

本示例模板不支持使用编译器进行编译。使用下列方式编译前，需要安装最新的 TeXLive 发行版。

### VSCode 用户

安装 “LaTeX Workshop” 后，选择 `Recipe: latexmk (xelatex)` 编译即可，并在设置中将 `latex-workshop.latex.recipe.default` 改为 `lastUsed` 以一直使用该选项编译。

### TeXStudio 用户

在TexStudio的菜单栏中，Options-Configure TeXstudio界面中，修改以下两处：

Commands-Latexmk一项修改为`latexmk -silent -synctex=1 -xelatex %`

Build-Default Compiler一项修改为`txs:///latexmk`

<details>

<summary>展开配置</summary>

<img src="https://user-images.githubusercontent.com/84025388/142163308-3d31f905-af78-40cb-bff1-851cdab04c87.png" width=500px/>

<img src="https://user-images.githubusercontent.com/84025388/142163346-63ec7b7e-932f-44c5-90c4-3b35e435545d.png" width=500px/>

</details>

## 致谢

* 感谢 [@sjtug](https://github.com/sjtug) 提供的 [SJTUThesis](https://github.com/sjtug/SJTUThesis) 模板。

## 软件许可证

上海交通大学校徽校名图片（`sjtu-vi-logo-blue.pdf` 等）的版权归上海交通大学所有。

`sjtureport.cls` 文档类与相关附属文件使用 [LPPL](https://www.latex-project.org/lppl.txt) 授权。

其他部分使用 [MIT LICENSE](LICENSE) 授权。
