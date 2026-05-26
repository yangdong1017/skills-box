# skills-box

个人  Skills 收藏仓库，用来存放标准化、可搬运、带脚本的 skill 包。


## 当前收录

| Skill | 路径 | 说明 |
|---|---|---|
| Claude.skill | `skills/Claude.skill/` | Anthropic 官方 Skill Creator，用于创建、修改、评估和优化。 |

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
