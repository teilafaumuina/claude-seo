# Teila's fork of claude-seo

Upstream: https://github.com/AgriciDaniel/claude-seo
Forked at: 468ed5b (v2.6.2), 2026-11-21

## Changes from upstream

| File | Change | Why |
|---|---|---|
| `skills/seo/SKILL.md` | Removed the "Community Footer" section | Promo block was being appended to client deliverables |
| `.claude-plugin/marketplace.json` | Marketplace `name` is `teila-claude-seo` | So it installs alongside, not over, the upstream marketplace name |

Keep this table current: it is the list of things to re-check after each upstream sync.

## Pull in upstream updates

```powershell
cd "$HOME\01 Personal\Agentic Systems\claude-seo"
git fetch upstream
git merge upstream/main
git push
claude plugin marketplace update teila-claude-seo
claude plugin update claude-seo@teila-claude-seo
```

If the merge reports a conflict, it is almost always in one of the two files above: keep upstream's new text and re-apply our change.
