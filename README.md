# fo-skill

fo导内容工作台。一套专为抖音情感内容创作者设计的 Claude Code Skill，覆盖写稿、审稿、内容诊断、开头优化、复盘五个场景。

---

## 工具箱

| Skill | 做什么 |
|---|---|
| `/fo` | 主入口，自动路由到对的工具 |
| `/fo-write` | 写稿助理，六步流程写逐字稿 |
| `/fo-content` | 内容诊断 + 审稿，三维评分+禁用句式扫描 |
| `/fo-hook` | 开头优化，诊断+生成10+条开头方案 |
| `/fo-retrospective` | 复盘助理，对照爆款规律提炼新发现 |

---

## 工作流

```
fo-content（选题怎么做）
    ↓
fo-write（写逐字稿）
    ↓ 开头有问题
fo-hook（优化开头）
    ↓ 写完
fo-content（审稿评分）
    ↓ 发布后
fo-retrospective（数据复盘）
```

---

## 安装

```bash
git clone https://github.com/folove66/fo-skill.git /tmp/fo-skill && cp -r /tmp/fo-skill/skills/fo* ~/.claude/skills/ && mkdir -p ~/.claude/知识库 && cp -r /tmp/fo-skill/知识库/* ~/.claude/知识库/ && rm -rf /tmp/fo-skill
```

安装后在 Claude Code 中输入 `/fo` 即可启动。
