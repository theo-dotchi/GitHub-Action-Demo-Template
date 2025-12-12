## Agenda

### 1 What is GitHub Action ? (1min)
### 2 Why it can improve your organization (2min)
### 3 How does it automate workflow ? (2 min)
### 4 Demo (Setup, Marketplace, Custom action, Debugging) (12min)
### 5 Conclusion (2min)

## GitHub Actions — Automating Developer Workflows

GitHub Actions is a platform that automates developer workflows directly where the code lives.  
Instead of relying on external tools, teams define workflows as code that react automatically to events such as pull requests, commits, or releases. From continuous integration and delivery to testing, security checks, and operational tasks, GitHub Actions enables teams to standardize and automate the entire software delivery lifecycle. By embedding automation inside GitHub itself, developers receive fast feedback, organizations enforce consistent practices, and teams can deliver changes faster and more safely—without changing how developers work.

Or a slightly more expressive version:

[ Merged Code ]
      ↓
[ Automated Tests ]
      ↓
[ Build & Package ]
      ↓
[ Deployment ]


> [!NOTE]
> GitHub action is a platform that automates developpement workflow, not only CI/CD



#### DORA Metrics (plus Security)

| Metric | What it measures | low performer | high performer| How to measure in practice |
|---|---|---:|---:|---|
| **Lead time for changes** | Time from code committed to code running in production | **Months** | **< 1 day** | PR merge → deploy timestamp (from CI/CD + change management) |
| **Deployment frequency** | How often you deploy to production | **Once per month (or less)** | **On-demand / multiple times per day** | Count production deployments per day/week |
| **Change failure rate** | % of deployments causing incidents / rollbacks / hotfixes | **31–45%** | **0–15%** | Incidents linked to deploys + rollback/hotfix tags |
| **Mean time to recovery (MTTR)** | How fast you restore service after an incident | **Weeks to months** | **< 1 hour** | Incident start → service restored time |
| **Security (recommended add-on)** | How quickly and reliably you remediate vulnerabilities and prevent regressions | **Vulns linger for months; fixes are ad-hoc** | **Fix SLAs met; automated detection + policy gates** | Time-to-remediate (TTR), % repos with scanning enabled, vulnerable dependency age, secret exposure rate |

> Notes (DORA benchmarks): The “elite” vs “low” ranges above reflect commonly cited DORA performance categories.
```

