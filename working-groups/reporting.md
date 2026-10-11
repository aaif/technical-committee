# Working Group Monthly Reporting to the Technical Committee

* Status: FINAL
* Effective Date: 2026-06-01 

### Purpose

Establish a lightweight, predictable process for AAIF Working Groups (WGs) to report progress to the Technical Committee (TC) each month, prioritising asynchronous review over live presentations and using GitHub as the single source of truth.

### Process

Each WG submits a monthly progress report as a markdown file added to its own repository under a `reporting/` directory. Files **must** follow the *case-sensitive* naming convention `YYYY-MM-report.md` (e.g. `reporting/2026-05-report.md`) to keep history sortable and discoverable, and to aid automation.  

The report is opened as a pull request against the WG's repo, with the TC (or a designated TC GitHub team) added as reviewers. To aid automation, you **must** adhere to this format:

* PR title: `[Report] <YYYY-MM>`  
* PR label `monthly-report`

Reports are due by the **last business day of each month**; the review window closes **7 calendar days later**.

TC members review and comment directly on the PR. Once the review window closes — or once the TC has signed off, whichever is sooner — the WG chair merges the PR. The merged file becomes the canonical record of that month's progress.

### Report Template

Each report should be short and scannable, covering:

* **Summary** — 2–3 sentence overview of the month  
* **Progress against objectives** — what shipped, what advanced  
* **Blockers and risks** — anything the TC should be aware of  
* **Decisions needed from the TC** — explicit asks, if any  
* **Next month's focus** — top 2–3 priorities  
* **Metrics / links** — relevant PRs, issues, releases, meeting notes

A template will live at `reporting/TEMPLATE.md` in each WG repo.

### Async by Default, Live When Needed

Async review is the default. The TC may, at its discretion, request that a WG present its report live at a TC sync call when:

* the report surfaces a material blocker, risk, or cross-WG dependency  
* a decision is requested that benefits from real-time discussion  
* the TC has substantive questions that PR comments aren't resolving efficiently

Live presentations are the exception, not the norm. When requested, the CTO will notify the WG chair at least 5 business days before the relevant TC sync.

### Escalation

If a WG misses two consecutive monthly reports without prior notice to the TC chair, the TC will schedule a live check-in with the WG at the next available sync.

### Benefits

* **Low overhead for WGs** — one markdown file, one PR per month  
* **Transparent and auditable** — all reports live in public repos with full review history  
* **Respects time zones and schedules** — async-first accommodates a distributed contributor base  
* **Preserves TC flexibility** — live presentations remain available when they add real value
