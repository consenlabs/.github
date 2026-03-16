# consenlabs/.github

Organization-wide default [community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file) for **Consenlabs** repositories.

These templates are automatically inherited by all repos under the `consenlabs` org, unless a repo provides its own version.

---

## What's Included

### Issue Templates (`.github/ISSUE_TEMPLATE/`)

| Template | Type | Description |
|----------|------|-------------|
| 🐞 [Bug Report](/.github/ISSUE_TEMPLATE/bug.yml) | Bug | 报告缺陷，含平台、设备、复现步骤等结构化字段 |
| 🚨 [Incident Report](/.github/ISSUE_TEMPLATE/incident.yml) | Bug | 生产事故报告，含根因分析、影响评估、修复方案 |
| 📖 [Story](/.github/ISSUE_TEMPLATE/story.yml) | Story | 用户故事，遵循 INVEST 原则，含功能/非功能/性能验收标准 |
| 📝 [Task](/.github/ISSUE_TEMPLATE/task.yml) | Task | 通用任务，含背景 (WHY)、方案 (HOW)、完成定义 |

> Blank issues are disabled ([config.yml](/.github/ISSUE_TEMPLATE/config.yml)) — all issues must使用上述模板之一。

### Pull Request Template

[`pull_request_template.md`](/pull_request_template.md) — 统一 PR 模板，包含：
- **Summary** — 一句话说清 Why & What
- **Testing** — Reviewer 验证 checklist
- **AI 参与度** — 标注 AI-Generated / AI-Assisted / Human-Written

### Legacy PR Templates (`docs/PULL_REQUEST_TEMPLATE/`)

历史遗留的前后端分离模板，可按需手动引用：

| Template | Command |
|----------|---------|
| Backend | `curl -o .github/PULL_REQUEST_TEMPLATE.md https://raw.githubusercontent.com/consenlabs/.github/main/docs/PULL_REQUEST_TEMPLATE/be-pull-request-template.md` |
| Frontend | `curl -o .github/PULL_REQUEST_TEMPLATE.md https://raw.githubusercontent.com/consenlabs/.github/main/docs/PULL_REQUEST_TEMPLATE/fe-pull-request-template.md` |

> **注意**：根目录的 `pull_request_template.md` 已作为组织默认模板生效。上述 Legacy 模板仅在个别 repo 需要更详细的 Security Checklist 时使用。

---

## How It Works

GitHub 会按以下优先级查找 community health files：

1. **Repo 自身** — `.github/` 或根目录下的模板
2. **Org `.github` repo** — 即本仓库，作为 fallback

因此，如果某个 repo 需要自定义模板，只需在该 repo 中创建同名文件即可覆盖。

## Contributing

修改模板请提交 PR 到本仓库。变更会自动应用到所有未自定义模板的 consenlabs repos。
