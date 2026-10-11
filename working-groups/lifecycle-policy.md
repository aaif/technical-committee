# **AAIF Working Group Lifecycle Policy**

* Status: FINAL
* Revision: 2
* Effective Date: 2026-10-02 

## **Purpose**

This policy sets out how AAIF Working Groups (WGs) are proposed, launched, run, renewed and closed. It aims to keep the WG portfolio healthy and relevant with as little process as possible: a healthy WG should spend a few hours a year on it, and the TC one short review per WG per year.

It works alongside two things that already exist: the [WG proposals repo](https://github.com/aaif/working-group-proposals), where new WGs are proposed, and the [WG Monthly Reporting](reporting.md) process, which supplies the health signals this policy relies on. It borrows from CNCF TAG governance, the Kubernetes and OpenSSF WG lifecycles, W3C's time-bound charters and the Apache Attic.

**MUST**, **SHOULD** and **MAY** are used as defined in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

## **The lifecycle at a glance**

**Proposal approved → Sandbox → Active** (renewed every 12 months) **→ Concluded**. A Sandbox WG that doesn't take off goes straight to Concluded, and a Concluded WG can be revived back into Sandbox.

| Stage | What it means | Duration |
| :---- | :---- | :---- |
| **Sandbox** | Approved, meeting, and writing its charter. | 6 weeks; may be extended once by up to 6 weeks |
| **Active** | Chartered and delivering against its objectives. | 12-month charter periods, renewed each year |
| **Concluded** | No longer operating. Its record is preserved and it can be revived. | Open-ended |

Proposals that haven't been decided yet are tracked on the proposals board, not as a WG stage.

## **Who can do what**

| Action | Who |
| :---- | :---- |
| Participate in a WG | Anyone |
| Propose a new WG or a revival | People from any AAIF member organization (Platinum, Gold, Silver or Associate) |
| Serve as a chair | People from Platinum, Gold or Silver member organizations |
| Vote in a contested chair selection | WG participants from Platinum, Gold or Silver member organizations |
| Approve lifecycle decisions | The TC |

Non-members with an idea for a WG are welcome to ask a member organization to sponsor the proposal.

### **How the TC decides**

Unless this policy says otherwise, TC decisions are made by **lazy consensus** on the relevant GitHub issue or PR: the decision passes if no TC member objects within 7 days. Any objection moves it to a vote, decided by a simple majority of all TC members. Three decisions always go to a vote:

* approving a new WG (also subject to Governing Board approval, per the current proposals process);  
* moving a WG to Concluded when its chairs haven't asked for it;  
* removing a chair (two-thirds of all TC members).

## **1\. Proposing a WG**

First check whether the work fits inside an existing WG as a workstream (see Section 4). New WGs are for long-lived problem domains; tightly scoped or time-boxed efforts SHOULD be workstreams.  
Proposals are submitted through the [issue form](https://github.com/aaif/working-group-proposals/issues/new?template=working-group-proposal.yml) in the proposals repo. Be clear and succinct, it helps the TC read every proposal properly. A proposal MUST include:

* **Problem statement:** the gap in the agentic AI ecosystem, and why no existing AAIF WG or external body already covers it.  
* **Scope and first deliverables:** what the WG will and won't cover, and what it expects to ship in its first year.  
* **Overlap:** adjacent AAIF WGs and external bodies (for example W3C, IETF, OpenSSF, CNCF or OWASP), and how the WG will coordinate with them rather than compete.  
* **Leadership:** a proposed chair and co-chair from two different member organizations.  
* **Demand:** named people from at least three organizations who commit to taking part.

AAIF staff check the proposal is complete, then the TC reviews it asynchronously on the issue. The TC SHOULD decide within 8 weeks of a complete submission. It can approve (the WG enters Sandbox), ask for changes, redirect the work (for example into an existing WG as a workstream), or decline. Every outcome comes with written reasons on the issue.

## **2\. Charters**

A charter is a single page that the WG writes and the TC approves. It MUST contain:

* **Mission:** one or two sentences on the long-term vision.  
* **Scope and out of scope.**  
* **12-month objectives:** concrete deliverables, each with a target date and a clear definition of done. At least one SHOULD be due within the first six months, because groups without near-term deliverables tend to stall in discussion.  
* **External relationships:** the outside bodies the WG expects to work with, and any formal liaison it wants the TC to approve (see Section 4).

The mission can stay the same for years; the objectives are rewritten every year at renewal. Paint the vision in a sentence, then commit to what you'll deliver in the next twelve months. No ten-year plans.  
Charters don't cover governance. This policy is the governance for every WG. A WG that needs to work differently MAY record the difference in its charter, with TC approval.

## **3\. Sandbox**

An approved WG starts in Sandbox. The TC assigns it an adopter, and AAIF staff set up its repo (with `charter/`, `reporting/` and `meeting-notes/` directories), meeting series and channels. The WG starts meeting and filing monthly reports straight away.  
Sandbox has one job: **agree the charter**. Within 6 weeks, the chairs open a PR adding the charter to the WG's repo, with the TC as reviewers. Writing it together in Sandbox, rather than in the proposal, means the people who actually show up own the plan.  
When the charter PR is ready (or at the 6-week mark), the TC adopter confirms the WG has been meeting with participants from at least three organizations, and the TC then:

* **approves the charter:** the WG becomes Active; or  
* **extends Sandbox** once, by up to 6 weeks, with specific asks; or  
* **moves the WG to Concluded:** the idea didn't find its footing. This is a normal, no-fault outcome.

## **4\. Active**

An Active WG MUST:

* meet at least monthly, in the open, and publish notes;  
* file monthly reports under the reporting process (these carry workstream status too);  
* keep its charter and README (chairs, meeting times, links) up to date.

It SHOULD mentor future chairs, so leadership can change hands without a gap.

### **Chairs**

* Every WG has two chairs from different member organizations, so meetings don't depend on one person and no single company runs the group.  
* Chairs are chosen by lazy consensus within the WG. If that's contested, the WG holds a vote of eligible participants (see "Who can do what"). The TC then confirms the chairs.  
* A chair's term matches the charter period (12 months) and is renewable. Chairs are reconfirmed as part of the annual renewal.  
* A chair MAY step down at any time and SHOULD propose a successor. The WG fills the seat the same way it chose the original chairs.  
* If a WG has no active chair for 30 days, the TC appoints an interim chair or moves the WG to Concluded.  
* The TC MAY remove a chair who is inactive or not meeting these responsibilities.

### **Working with other groups**

WGs have influence, not authority. Participants are encouraged to work with other AAIF WGs and outside bodies: attend their meetings, share drafts, invite speakers, build relationships.  Without TC approval, a WG MUST NOT:

* state an official AAIF position to an external body;  
* enter a formal liaison, memorandum of understanding or joint deliverable with an external body;  
* commit AAIF resources or funding.

### **Workstreams**

Workstreams are how a WG organizes focused, time-bound work (similar to CNCF initiatives):

* The chairs create and close them. No TC approval is needed.  
* Each has a named lead, a goal and a target date, as set by the chairs in consultation with the WG.
* Status goes in the WG's monthly report.  
* A workstream that makes no progress for a quarter SHOULD be closed or re-scoped.  
* Work that spans several WGs has one home WG that owns it and reports on it.

## **5\. Annual renewal**

Each charter runs for 12 months. Near the end of that period, the chairs open a renewal PR that:

* reports against the past year's objectives: what shipped, what slipped and why, and how participation has changed;  
* updates the charter with objectives for the next 12 months and any scope changes;  
* confirms the chairs for the next term.

The TC reviews it and recommends **renew**, **renew with changes** or **move to Concluded**. For a healthy WG, renewal is the expected outcome and happens by lazy consensus.  
The review measures each WG against the objectives it set itself, not against a common bar. A WG taking on a hard, multi-year problem is judged on whether it is making the progress it said it would.  
If a review runs late, the current charter stays in effect until it is done.

## **6\. When a WG is struggling**

Monthly health status (🟢 / 🟡 / 🔴) is the early-warning system. Amber and red are prompts for help first: facilitation, recruiting, narrowing scope, new chairs or a merge.  
A **lifecycle review** starts when any of these happens:

* 🔴 red for two consecutive months, or 🟡 amber for three;  
* three missed monthly reports (the reporting process already calls for a live check-in after two);  
* no WG meeting for 60 days;  
* no active chair for 30 days.

In a lifecycle review, the TC and chairs agree a recovery plan. If the WG hasn't recovered within 60 days, the TC MAY move it to Concluded. Triggers start a conversation; they never move a WG automatically.

## **7\. Concluded**

Every WG eventually concludes, and concluding isn't a failure. A WG moves to Concluded when:

* **its mission is accomplished** and it asks to close. This is the path to celebrate, and it SHOULD be recognized publicly;  
* **it merges** into another WG, which takes on its remaining work;  
* **it is no longer viable**, as decided by the TC at the end of Sandbox, at renewal, or after a lifecycle review.

### **Closing checklist**

The chairs own this list (or the TC if no chairs remain); AAIF staff handle the admin.

1. Publish a short final report in `reporting/`: outcomes, deliverables and lessons learned.  
2. Hand over anything still in use (specs, tools) to another WG, an AAIF project or an upstream body, or mark it clearly as unmaintained.  
3. Mark the README as Concluded with the date and reason, and announce it to the community.  
4. Archive the repo as read-only and close the meeting series and channels. Nothing is deleted.

### **Revival**

Any member MAY propose reviving a Concluded WG through the normal proposal process, using its old charter as a starting point. If approved, it restarts in Sandbox.

## **Roles**

| Role | Responsibilities |
| :---- | :---- |
| **TC** | Approves new WGs, charters, renewals, chair appointments and moves to Concluded. |
| **TC adopter** | The TC member who reviews a WG's monthly reports (see the reporting process). Sets health status, leads lifecycle reviews and makes the renewal recommendation. |
| **WG chairs** | Run meetings, file reports, keep the charter and README current, lead renewal and carry out the closing checklist. |
| **AAIF staff** | Check proposals for completeness, set up and archive repos, meetings and channels, and keep the list of WGs current. |

## **Transition for existing WGs**

* Within 30 days of this policy being adopted, each existing WG tells its TC adopter which stage it's starting in: **Active** if it has an approved charter, **Sandbox** if its charter isn't finished (the 6-week clock starts on adoption), or **Concluded** if it would rather close. The TC confirms by lazy consensus.  
* An Active WG's first renewal falls 12 months after its charter was approved. Current chairs' terms run until then.  
* Existing charters don't need rewriting now. They move to the one-page format at first renewal.
