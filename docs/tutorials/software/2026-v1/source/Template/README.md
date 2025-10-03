# 智能车创新社新成员指导手册

## 文件说明

- `main.tex` - 主 LaTeX 文档
- `avatar.jpg` - 社团头像图片
- `README.md` - 本说明文件

## 编译要求

### 必需软件
1. **TeX Live** 或 **MiKTeX** (LaTeX 发行版)
2. **XeLaTeX** 引擎 (支持中文)

### 必需包
```latex
ctex          % 中文支持
geometry      % 页面布局
graphicx      % 图片支持
tikz          % 绘图
tcolorbox     % 彩色框架
minted        % 代码高亮 (需要 Python pygments)
fontawesome5  % 图标字体
```

## 编译方法

### 编译命令
```bash
xelatex -shell-escape main.tex
xelatex -shell-escape main.tex  # 生成目录需要编译两次
```

## 自定义说明

### 修改个人信息
在 `main.tex` 中搜索并修改：
- 作者姓名
- 联系方式
- 社团信息

### 添加内容
文档采用模块化设计，可以轻松添加新章节：
```latex
\section{新章节标题}
\subsection{子章节}
内容...
```

### 自定义样式
- `smartblue` - 主题蓝色
- `smartorange` - 强调橙色
- `smartgray` - 辅助灰色

### 特殊框架
- `\begin{tipbox}` - 提示框
- `\begin{warningbox}` - 警告框
- `\begin{codebox}` - 代码框

## 输出效果

编译成功后会生成：
- 专业封面（包含头像）
- 完整目录
- 格式化正文
- 彩色代码框和提示框

## 注意事项

1. 确保 `avatar.jpg` 在当前目录
2. 首次编译可能需要下载字体包
3. 使用 `-shell-escape` 参数启用 minted 代码高亮
4. 编译两次以正确生成目录和交叉引用