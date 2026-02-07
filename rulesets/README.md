# GitHub Rulesets — secondordereffects org

Reference rulesets for branch protection across all 3 repos. Apply via GitHub UI: **Settings → Rules → Rulesets → Import**.

| File | Repo | Key Rules |
|------|------|-----------|
| `content-main.json` | `secondordereffects/content` | 1 approval required, status check (`trigger`), linear history, no force push, no delete |
| `engine-main.json` | `secondordereffects/secondordereffects.github.io` | 0 approvals (solo dev), status check (`build-deploy`), linear history, no force push, no delete |
| `brand-main.json` | `secondordereffects/brand` | 1 approval required, linear history, no force push, no delete, no status checks |

All rulesets bypass for **OrganizationAdmin** so the org owner can push directly to main. Everyone else must go through a PR.
