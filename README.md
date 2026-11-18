# AI四库全典 · Skill

《AI四库全典》四部四十八卷、255.9 万字人工智能百科的离线全文语料与检索技能。
装上它，Agent 就能在不联网、不调大模型 API 的情况下检索全书、给出带卷次章节的出处，并可直接打开离线 WEB 阅读器。

## 内容

- `assets/corpus/vol-001.md` … `vol-048.md`：48 卷完整正文（经 12 / 史 12 / 子 12 / 集 12）
- `references/catalog.md`：四部 48 卷、约 2571 节完整目录
- `scripts/search.py`：零依赖中文全文检索（AND 多词、按部/卷过滤、JSON 输出）
- `assets/reader/`：离线 WEB 阅读器，`index.html` 双击即用（全文分 4 片内嵌、目录/检索/批注/夜读）

## 安装

### ClawHub / OpenClaw

```bash
openclaw skills install ai-siku-quan-shu
# 或
clawhub install ai-siku-quan-shu
```

### WorkBuddy

把本目录复制到 `~/.workbuddy/skills/ai-siku-quan-shu/`（用户级）或项目的 `.workbuddy/skills/`（项目级）。

## 用法示例

```bash
python3 scripts/search.py "RAG 向量数据库" --vol 子
python3 scripts/search.py "深蓝 卡斯帕罗夫" --limit 5
python3 scripts/search.py --read vol-031 --lines 120
python3 scripts/search.py --list
```

Agent 触发后应先检索再作答，引用格式：
`（出处：子部·第7卷《检索增强 RAG 与知识工程》· 章节标题）`

## 许可

ClawHub 上发布的技能统一采用 MIT-0：可自由使用、修改、再分发，含商用，无需署名。
本仓库沿用同一许可。语料内容由学来学去学习社 AI 学伴团编撰，引用请标注卷次章节。

## 维护

开发工具：上海巧未来人工智能科技有限公司
主编：学来学去学习社 AI 学伴团
