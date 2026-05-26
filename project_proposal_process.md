**AAIF Project Proposal Process**

*Operating procedure for the Agentic AI Foundation*

**Version**: v0.2

# **1\. Purpose**

This document describes how projects are proposed, reviewed, approved, and onboarded into the Agentic AI Foundation (AAIF).

The [AAIF Project Lifecycle Policy](https://github.com/aaif/project-proposals/blob/main/governance/project-lifecycle-policy.md) remains the governing authority for lifecycle stages, admission criteria, and annual review. This procedure is the operating workflow that implements that policy.

# **2\. Process at a Glance**

The process has six sequential steps, plus one parallel step that must be completed before the Technical Committee vote, and one optional on-demand sub-step (a live TC presentation, scheduled only if a TC member requests one).

Each step is also classified by its mode of execution - whether it happens live (e.g., in a meeting, on a video call) or offline (e.g., asynchronously via email, GitHub, or LFX voting tools). The process is deliberately designed to default to offline execution wherever possible, recognising that the Technical Committee is geographically distributed and that submission volume makes per-project live meetings expensive at the committee level.

A guiding principle of this process is that the Foundation guarantees a meaningful engagement bar on every submission - a minimum number of TC members must engage with the proposal before it can advance to a vote - rather than guaranteeing that every project has a single named champion. This shift trades depth (one enthusiastic supporter) for breadth (several engaged committee members) and is intended to surface concerns earlier and reduce the risk of submissions being nodded through procedurally. A TC supporter role still exists, but is invoked only on demand if the engagement bar is not met (see Step 2).

| Step | Owner | Mode | Category | Tools Used |
| :---- | :---- | :---- | :---- | :---- |
| 1\. Initial intake | CTO (assisted by intake agent) | Offline | Intake & review | Notified via intake agent that conducts initial checks then alerts CTO \+ TC chairs via email \+ Discord. |
| 2\. TC Q\&A window | Technical Committee | Offline | Intake & review | TC notified email \+ Discord, further engagement via GH notifications on ticket. |
| Presentation *(on demand only)* | Project submitter | Live | Intake & review | Scheduled via PMO, status reflected on ticket |
| Contributor paperwork *(parallel)* | Project submitter | Offline | Parallel step | Scheduled via PMO, status reflected on ticket |
| 3\. TC vote | Technical Committee | Offline | Voting gate (absolute majority) | Voted on using LFX Vote, outcome reflected on ticket |
| 4\. GB approval | Governing Board | Offline | Voting gate (absolute majority) | Voted on using LFX Vote, outcome reflected on ticket |
| 5\. LF Legal formation | LF Legal / AAIF Staff | Offline | Legal & onboarding | Final paperwork sent via DocuSign to Submitter |
| 6\. Technical onboarding | Project submitter / LF IT | Offline | Legal & onboarding |  |

![][image1]

## **2.1. Automation**

As a general principle, the processes described should be automated as much as possible. It is the responsibility of the owner of each step to consider which components can and will be automated within that step.

This document will not attempt to mandate which components will be automated or attempt to describe how those components will be automated, as those implementation details are outside the scope of this document.

# **3\. Roles**

The process is deliberately limited to a small set of actors. Each plays a defined role at one or more stages.

| Role | Responsibility |
| :---- | :---- |
| **Project submitter** | Files the proposal, responds to TC questions on the GitHub issue during Step 2, presents to the TC if a presentation is requested, completes contributor paperwork, and executes technical onboarding. |
| **CTO** | Owns Step 1: screens submissions for completeness and fit, conducts the smoke test (assisted by the intake agent), gathers TC chair input via the GitHub issue, and prepares the TC brief. Approves Q\&A window extensions in Step 2, and triggers the on-demand TC supporter mechanism if the engagement bar is not met. |
| **Intake agent** | An automated agent that performs two functions on each new submission: a public technical compliance check (posted as a comment on the GitHub issue) and a private advisory review (delivered to the TC via a TC-only channel). Both outputs are advisory only; the CTO retains the final decision in Step 1 and the TC retains the final decision in Steps 2 and 3\. |
| **TC chairs** | Provide input on submissions during Step 1 via comments on the GitHub issue. If the engagement bar in Step 2 is not met, the chairs seek a TC supporter willing to champion the project; if none can be found, the submission is rejected. |
| **TC supporter**  *(on demand)* | A Technical Committee member appointed only when the Step 2 engagement bar has not been met. Represents the project within the TC, drives engagement on the GitHub issue, and champions the project through a restarted Q\&A window. If no TC member is willing to act as supporter, the submission is rejected. |
| **Technical Committee** | Engages with submissions during the Step 2 Q\&A window on the GitHub issue, may request a live presentation, and votes on admission and initial lifecycle stage by absolute majority in Step 3\. |
| **Governing Board** | Confirms organisational readiness and resource implications, and votes on admission by absolute majority. |
| **LF PMO** | Coordinates intake and scheduling, runs the GitHub issue record, and liaises with LF Legal and LF IT. Coordinates project onboarding. |
| **LF Legal** | Prepares and finalises the contribution agreement, technical charter, and trademark and asset transfers. |
| **LF IT** | Assumes repository ownership and executes the technical onboarding of project infrastructure. |

# **4\. Submission Requirements**

Proposals are submitted as a GitHub issue in the AAIF [project proposals repository](https://github.com/aaif/project-proposals). The issue is the official record for the submission from intake through closure. Each proposal must include:

* Project name, description, origin, and a statement of alignment with the AAIF mission.
* Licence (OSI-approved permissive or open specification), repository location, and issue tracker.
* Governance model, maintainers, and decision-making process.
* Evidence of adoption, external dependencies, and any infrastructure needs.
* Official communication channels, website, and any social accounts.
* Preferred initial lifecycle stage (Growth or Impact) per the AAIF Project Lifecycle Policy.

# **5\. The Process**

## **Step 1 - Initial intake**

**Owner:** CTO (assisted by intake agent)

Initial intake is a lightweight smoke test of the new project rather than a deep technical review. The CTO owns the step end to end, and the entire step is conducted offline on the GitHub issue - there is no scheduled meeting at this stage.

The smoke test covers:

* Completeness against the submission requirements in Section 4\.
* High-level fit with the AAIF mission and scope.
* Obvious red flags around licensing, governance, or community health.
* Whether the proposed lifecycle stage (Growth or Impact) appears defensible at first glance.

### **Intake agent**

The smoke test is supported by an automated intake agent. The agent performs two distinct functions on each new submission, with different audiences and different visibility:

**Technical compliance check (public)**

On submission of a new GitHub issue, the agent performs a mechanical compliance check against the submission requirements in Section 4 - verifying that all required fields are present, that the licence is OSI-approved or a recognised open specification, that linked repositories and issue trackers resolve, and that other structural requirements are met. The agent posts the results of this check as a comment on the GitHub issue, visible to the submitter and to anyone reading the issue. Submitters are encouraged to address any flagged gaps before the CTO completes the smoke test. This part of the agent's output is deliberately public so that the submitter has clear, actionable feedback on what to fix.

**Advisory review (private to the TC)**

Separately, the agent produces a subjective advisory review covering its assessment of mission alignment, governance maturity, the credibility of adoption evidence, community-health signals, and any concerns it would flag for the wider Technical Committee. This review is not posted on the public GitHub issue. It is delivered through a TC-only channel - either a private TC repository, an LFX-managed discussion, or another mechanism agreed by the TC - and is visible only to TC members and AAIF Staff.

The advisory review is kept private for two reasons. First, it is judgment-laden rather than mechanical, and exposing it to the submitter would create friction over an opinion the submitter cannot meaningfully respond to in the same way they can to a missing-field check. Second, a public advisory review would become a gameable target - submitters would tune proposals to satisfy the agent rather than the TC. The advisory review exists to give the TC an additional perspective ahead of the Step 2 Q\&A window, not to score the submission.

In both functions, the agent's output is advisory only - the CTO retains the final decision in Step 1, and the TC retains the final decision in Steps 2 and 3\. The agent does not vote and does not gate the process.

### **TC chair input**

As part of initial intake, the CTO solicits input from the two TC chairs by tagging them on the GitHub issue. Their responses are left as comments on the issue, which keeps a transparent, durable record of TC input alongside the proposal itself. The CTO does not block on a chair response indefinitely.

### **Outcome of Step 1**

If the proposal is incomplete or out of scope, the CTO records the reason in the GitHub issue and either requests clarification or closes the issue with feedback. Out-of-scope submissions may be closed immediately.

If the proposal passes the smoke test, the CTO prepares a short brief summarising mission alignment, licence, governance, adoption evidence, proposed lifecycle stage, the intake agent's advisory review (or a summary of it), any input gathered from the TC chairs, and any open questions. The brief is posted on the GitHub issue and circulated to the Technical Committee. This opens the Step 2 Q\&A window.

The smoke test is intentionally not a substitute for the TC's review in Step 2 or its vote in Step 3\. Its purpose is to filter out clearly out-of-scope or incomplete submissions early, and to surface any material concerns the chairs would want flagged in the brief.

## **Step 2 - TC Q\&A window**

**Owner:** Technical Committee    **Mode:** Offline (GitHub issue)

Once the CTO has posted the Step 1 brief on the GitHub issue, a fixed Q\&A window. During this window, any TC member may ask questions on the issue, and the project submitter responds in-thread. The Q\&A thread becomes the durable record of the committee's review of the proposal.

### **The engagement bar**

Before the Q\&A window can close and the proposal advances to a vote, a minimum of four TC acknowledgments must be recorded on the GitHub issue. An acknowledgment is any of the following: a substantive question, a comment indicating the member has reviewed the proposal and has no questions, or an explicit “approval reaction” on the brief comment. Acknowledgments from the TC chairs count, but acknowledgments from the project's TC supporter (if one has been appointed under the on-demand mechanism below) do not, since the supporter is by definition already engaged.

If the engagement bar has not been met by the end of the Q\&A window, the window does not auto-close - the on-demand supporter mechanism (below) is triggered instead. Silence is not treated as approval.

### **Extensions**

If healthy discussion is still active on the GitHub issue at the end of the Q\&A window, and the proposal is not yet ready either to go to vote or to schedule an optional presentation, the window may be extended. Either the project submitter or any TC member may request an extension by leaving a comment on the issue. The CTO approves the extension.

Extensions are five business days each, and are limited to one extension per project to avoid the window itself becoming a scheduling problem. Acknowledgments and questions gathered during the original window carry over into the extended window.

Extensions are only available while the engagement bar is on track to be met - they exist to give a productive discussion more time to conclude, not to wait for engagement that has not materialised. Once the on-demand TC supporter mechanism (below) has been triggered, no further extensions are available, since the supporter window is itself the remediation.

### **Optional presentation**

At any point during the Q\&A window or any extension, any TC member may request a live presentation from the submitter by saying so on the GitHub issue. A single request is sufficient - the bar is deliberately low so that any TC member who feels a live conversation would help can trigger one without negotiation.

If a presentation is requested, the submitter presents at the next scheduled TC meeting. The standard format is a ten-minute presentation followed by ten to fifteen minutes of questions, focused on fit, governance maturity, community health, and the proposed lifecycle stage. Step 3 (the TC vote) opens after the presentation.

If no presentation is requested by the close of the Q\&A window (including any extension), and the engagement bar has been met, the proposal advances directly to Step 3\.

### **On-demand TC supporter**

If the engagement bar is not met by the close of the Q\&A window (including any extension), the CTO asks the TC chairs to identify a TC supporter for the project. The supporter is a Technical Committee member willing to represent the project within the TC, drive engagement on the GitHub issue, field questions from other members, and champion the project to the rest of the TC.

If a supporter is found, they are named in the GitHub issue and the Q\&A window restarts under their stewardship. The engagement-bar and presentation rules above apply again to the restarted window.

If no TC member is willing to act as supporter, the CTO closes the GitHub issue with a documented rationale and the submission is treated as rejected. The submitter may reapply after three months under the same conditions as a Step 3 rejection. The absence of a willing supporter is itself a meaningful signal: if not one of TC members will champion the project after a full Q\&A window, that is a clear indication the project is not ready for AAIF or is a poor fit for the Foundation.

This on-demand mechanism is preferred over a default requirement that every project have a TC supporter named up front. The role exists as a remediation mechanism for low-engagement submissions rather than as a coordination cost paid on every submission.

## **Parallel - Contributor paperwork**

**Owner:** Project submitter, supported by AAIF PMO

If a project passes Step 1, , AAIF PMO will initiate the project formation workstream with LF Legal in parallel with Step 2\. A draft contribution agreement and technical charter are prepared and shared with the submitter and their legal counsel for review. The submitter must return agreed documents, execution-ready, before the GB vote opens in Step 5\. This avoids delays later in the process and gives the GB confidence that a yes vote leads directly to execution.

## **Step 3 - TC vote**

**Owner:** CTO and Technical Committee

The TC conducts an asynchronous vote in LFX over seven days. The vote opens at the close of the Q\&A window if no presentation was requested, or immediately following the optional presentation if one was held. Admission requires an absolute majority of all TC members, and the vote includes a recommendation on the initial lifecycle stage (Growth or Impact).

The TC produces one of three outcomes:

* Approval for referral to the Governing Board.
* Conditional approval identifying specific items that must be resolved before the project is treated as admitted.
* Rejection with a documented rationale. A rejected submitter may reapply after three months, provided meaningful improvements have been made.
* CTO updates the submission accordingly. 

## **Step 4 - GB vote**

**Owner:** Governing Board

Projects approved by the TC are referred to the Governing Board, which conducts an asynchronous vote over seven calendar days. The GB confirms organisational readiness, resource implications, and the Foundation's willingness to accept the project under the proposed terms and lifecycle stage. Approval requires an absolute majority.

Where the project repository runs CI on GitHub Actions or creates another recurring cost, the GB also confirms that AAIF is prepared to assume that obligation as part of its vote.

## **Step 5 - Finalise Legal Paperwork**

**Owner:** LF Legal, Project Submitter and AAIF PMO

Following GB approval, LF Legal, LF PMO, and Project Submitter execute the contribution agreement, technical charter, and transfer of trademarks and other required project assets. The Project Submitter has one week to sign the legal documents after GB approval or the offer is rescinded. The Linux Foundation performs a licence scan as part of this step. 

## **Step 6 - Technical onboarding**

**Owner:** Project submitter, LF IT, and LF PMO

Within four weeks of execution of the contribution agreement, the submitter,LF IT, and LF PMO complete the following:

* Implement the approved governance structure in the project repository (GOVERNANCE.md and technical charter).
* Transfer GitHub repository ownership to the Linux Foundation, or grant LF IT administrative control, and migrate into LF-managed infrastructure where required.
* Provide credentials and administrative access for the project website and official social media accounts to LF IT.

The GitHub issue is closed as Approved once onboarding is complete. 

# **6\. Initial Lifecycle Stage**

Every admitted project is assigned an initial lifecycle stage. The TC recommends the stage as part of its vote, and the GB confirms it on approval.

* **Growth** - for projects that show clear promise but still need mentorship, governance maturation, or contributor growth.
* **Impact** - for projects that already demonstrate substantial adoption, durable governance, diverse maintainership, and an established release cadence.

Admitted projects remain subject to the annual review process set out in the AAIF Project Lifecycle Policy.

# **7\. The Approval Gate**

A project is admitted to AAIF only when all five of the following are true:

* The proposal meets the submission requirements in Section 4\.
* The Technical Committee has approved the project by absolute majority.
* The Governing Board has approved the project by absolute majority.
* Contributor paperwork, the contribution agreement, and the technical charter are executed, and required assets are transferred to the Linux Foundation.
* Technical onboarding is complete.

**No public announcement is made before all five conditions are met.**

# **8\. Visibility**

[A dashboard](https://github.com/orgs/aaif/projects/1) is available where all stakeholders can quickly and clearly see where each submission is in the process.

[image1]: project_proposal_process.png
