# digit-data

<!-- [Codex] 公开发布版 1.0.0，2026-10-14。 -->

将本地 PDF 论文集整理为可持续维护的 **Markdown 文献 Wiki**，并按需要生成可离线浏览的研究方法图谱。

## 能做什么

- 从论文原文提取研究问题、方法、结果、图表和证据边界。
- 以单篇 Markdown 为唯一内容来源，维护索引、主题和论文关系。
- 按需核对发表年份、venue、DOI与正式发表状态。
- 指导模型生成搜索、年份筛选、详情卡片、模型图放大及键盘交互。
- 区分论文原图与 Wiki 示意、作者结论与整理者的横向判断。
- 增量更新已有资料库，检查链接、筛选状态和空结果提示。

## 安装

将完整仓库放入 Codex 个人技能目录，保持目录名为 `digit-data`。例如 Windows PowerShell：

```powershell
git clone https://github.com/qiujiu123/digit-data.git "$env:USERPROFILE/.codex/skills/digit-data"
```

若使用自定义技能目录，调整目标位置；已有同名目录时先检查和保留自己的修改。技能未显示时重新打开聊天或重启应用。

## 使用示例

```text
使用 $digit-data，把当前项目的 PDF 论文整理为 Markdown 文献 Wiki，保留出处和证据边界，并生成离线方法图谱。
```

```text
使用 $digit-data，增量纳入新论文，更新年份排序、方法分组和交互卡片，检查搜索、年份筛选和空结果状态。
```

## 仓库范围

这是一个**说明型技能**，包含工作流、质量标准和单篇论文模板。它不附带 PDF 解析器、预制网页生成器、论文数据集或已经整理好的文献库。实际生成脚本与页面由使用该技能的模型结合用户项目创建；所需阅读、联网与浏览器能力由运行环境提供。

Markdown 是内容来源，网页数据是生成物；不会把语法检查当作浏览器交互已经通过。不能确认的论文数字、图像身份或出版信息必须明确标注。

## 文件

- [SKILL.md](SKILL.md)：技能入口与质量检查。
- [references/wiki-schema.md](references/wiki-schema.md)：单篇论文结构、网页卡片映射、更新原则。
- [agents/openai.yaml](agents/openai.yaml)：技能显示与调用提示。
- [CHANGELOG.md](CHANGELOG.md)：公开版本修改记录。

采用 [MIT License](LICENSE)，许可范围仅为本仓库内容；使用者提供的论文及图片保留各自的权利和许可。
