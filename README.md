# skills-box

个人  Skills 收藏仓库，用来存放标准化、可搬运、带脚本的 skill 包。


## 当前收录

| Skill | 路径 | 说明 |
|---|---|---|
| Claude | `skills/Claude/` | Anthropic 官方 Skill Creator，用于创建、修改、评估和优化。 |
| dunya-pyq | `skills/dunya-pyq/` | 渡鸦科技社朋友圈文案引擎，用于生成、诊断、重写朋友圈和赛道快查。 |
| tongjincheng | `skills/tongjincheng/` | 童锦程视角关系分析 skill，用于暧昧、聊天、恋爱和人际关系建议。 |



## 使用方式

克隆全部仓库：

```bash
git clone https://github.com/yangdong1017/skills-box.git
```

复制需要的 skill 目录到目标 Claude Code skills 目录或项目目录中使用。

例如：

```text
skills/Claude/
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
