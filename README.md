# skills-box

个人 Claude Skills 收藏仓库，用来存放标准化、可搬运、带脚本的 skill 包。

## 仓库定位

这个仓库不是分类目录，也不是教程合集，而是一个私人 skill 包仓库。

每个 skill 都应当作为一个独立目录存在，目录内保留完整的 `SKILL.md`、脚本、素材、引用资料和许可证等文件，方便后续直接复制、同步、安装或二次改造。

## 当前收录

| Skill | 路径 | 说明 |
|---|---|---|
| Claude.skill | `skills/Claude.skill/` | Anthropic 官方 Skill Creator，用于创建、修改、评估和优化 Claude skills。 |

## 标准目录结构

```text
skills-box/
  README.md
  skills/
    Claude.skill/
      SKILL.md
      scripts/
      agents/
      references/
      assets/
      eval-viewer/
      LICENSE.txt
```

单个 skill 推荐保持如下结构：

```text
skills/<SkillName>/
  SKILL.md          # skill 主说明与触发规则
  scripts/          # skill 依赖脚本
  assets/           # 素材、模板或静态资源
  references/       # 参考资料、schema、规则文档
  agents/           # 子 agent 定义，如有
  LICENSE.txt       # 许可证，如有
```

## 使用方式

克隆仓库：

```bash
git clone https://github.com/yangdong1017/skills-box.git
```

复制需要的 skill 目录到目标 Claude Code skills 目录或项目目录中使用。

例如：

```text
skills/Claude.skill/
```

## 收录原则

- 一个 skill 一个独立目录。
- 保留原始 `SKILL.md` 和配套脚本。
- 不拆散 skill 包内部结构。
- 不按分类重组目录，避免破坏可搬运性。
- 修改第三方 skill 时，优先保留许可证和来源信息。

## 维护规则

新增 skill 时，直接放入：

```text
skills/<SkillName>/
```

如果 skill 来自压缩包，优先完整解压后再检查是否存在：

```text
SKILL.md
scripts/
LICENSE.txt
```

确认结构完整后再提交。