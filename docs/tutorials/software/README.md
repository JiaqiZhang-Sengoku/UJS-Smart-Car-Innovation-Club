# 软件组教程

本目录包含智能车社团软件组的历届教程文档。

## 教程列表

### 2026届

- **[2026-v1](./2026-v1/)** - 软件组教程第一版
  - 📄 [PDF文档](./2026-v1/TutorialForSoftwareTeamV1.pdf)
  - 📂 [LaTeX源码](./2026-v1/source/)
  - ✍️ 贡献者：[@xcmb-haochi](https://github.com/xcmb-haochi) (徐奕博 - 通信2402)

## 贡献指南

每届可以基于上一届的教程进行改进和更新：

1. 复制上一届的源码目录
2. 创建新的年份-版本目录（如 `2027-v1`）
3. 修改内容并重新编译PDF
4. 更新本README.md

## 编译说明

教程使用LaTeX编写，需要安装TeX发行版（如TeX Live或MiKTeX）。

编译命令：
```bash
cd source/TutorialForSoftwareTeamV1
lualatex TutorialForSoftwareTeamV1.tex
```
