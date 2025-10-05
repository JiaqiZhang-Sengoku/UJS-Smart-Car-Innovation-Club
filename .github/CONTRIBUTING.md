# 贡献指南

感谢你为江苏大学智能车创新社仓库做出贡献！

## 📝 提交规范

### 1. 添加个人信息

当你首次贡献时，请在README.md的"参与编写成员"部分添加你的信息：

```markdown
**🦉Contributors**: ... · [@你的姓名(专业+班级)](https://github.com/你的GitHub用户名)
```

**重要**：
- 必须包含GitHub主页链接，格式为 `[@姓名](GitHub链接)`
- 在其他地方提到自己时，也要添加可点击的GitHub链接

### 2. 仓库路径更新规范

⚠️ **当仓库主人改名或仓库地址变更时，必须同步更新以下位置：**

1. **README.md 中的badges**（第6行附近）
   ```markdown
   [![Contributors](https://img.shields.io/github/contributors/用户名/仓库名)]...
   [![Stars](https://img.shields.io/github/stars/用户名/仓库名)]...
   ```

2. **贡献者头像墙**（第22-24行附近）
   ```markdown
   <img src="https://contributors-img.web.app/image?repo=用户名/仓库名" />
   ```

3. **图片链接**（如2024学年的事件照片）
   ```markdown
   ![](https://github.com/用户名/仓库名/blob/main/...)
   ```

4. **Star History**（README末尾）
   ```markdown
   https://api.star-history.com/svg?repos=用户名/仓库名
   ```

5. **Git远程地址**
   ```bash
   git remote set-url origin git@github.com:用户名/仓库名.git
   ```

### 3. 文件组织规范

#### Tutorial（教程）文档
- **位置**：`docs/tutorials/[组别]/[年份-版本]/`
- **命名**：`YYYY-vN` （如 `2026-v1`）
- **内容**：
  - PDF文档放在版本根目录
  - LaTeX源码放在 `source/` 子目录
  - 在 `docs/tutorials/[组别]/README.md` 中添加索引

**示例**：
```
docs/tutorials/software/
├── README.md           # 软件组教程索引
├── 2026-v1/
│   ├── TutorialForSoftwareTeamV1.pdf
│   └── source/
└── 2027-v1/           # 后续版本
```

**README.md格式参考**：
```markdown
### 2026届

- **[2026-v1](./2026-v1/)** - 软件组教程第一版
  - 📄 [PDF文档](./2026-v1/xxx.pdf)
  - 📂 [LaTeX源码](./2026-v1/source/)
  - ✍️ 贡献者：[@姓名](GitHub链接) (专业班级)
```

#### 项目代码

- **位置**：README.md的"项目代码"部分
- **格式**：使用折叠区块，按届次 > 组别 > 具体项目组织

**格式参考**：
```markdown
<details>
<summary>第XX届全国大学生智能汽车竞赛</summary>

<details>
<summary>组别名称</summary>

**组员**：[@姓名](GitHub链接)（专业班级，角色）· 姓名（专业班级，角色）

- [**项目名称**](仓库链接) - 项目描述

</details>

</details>
```

### 4. Markdown 编写规范

- 参照已有内容的格式和风格
- 保持缩进和空行一致
- 链接格式统一使用 `[文字](URL)`
- 贡献者信息统一使用 `[@姓名](GitHub链接)（补充信息）` 格式

### 5. Commit 提交规范

提交信息要清晰描述改动内容，推荐格式：

- `添加xxx功能`
- `修复xxx问题`
- `更新xxx文档`
- `优化xxx结构`

## ❓ 问题反馈

如有疑问，请提交Issue或联系现任社团负责人。
