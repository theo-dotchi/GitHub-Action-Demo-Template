## Agenda

<img width="925" height="489" alt="image" src="https://github.com/user-attachments/assets/ee10a371-c8dc-4c4c-85de-e35751a07618" />

### 📖 

<img width="1388" height="624" alt="image" src="https://github.com/user-attachments/assets/c7b28407-5a2c-4a69-ac9d-608fd487e75d" />



> [!NOTE]
> GitHub action is a platform that automates developpement workflow, not only CI/CD
> - [Understanding GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions)
> - [Events that trigger workflows](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows)



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

