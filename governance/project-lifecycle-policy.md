# **Agentic AI Foundation Project Lifecycle Policy**
**Effective: March 18, 2026**

---

- ## Table of Contents

- [Overview](#overview)
- [Project Proposal Process](#project-proposal-process)
- [Stages: Definitions and Expectations](#stages-definitions-and-expectations)
- [Annual Review Process](#annual-review-process)

---

## Overview

This governance policy describes how an open technical project can formally join the Agentic AI Foundation (“AAIF”) via the Project Proposal Process. It describes the Stages a project may be admitted to and the criteria and expectations for each stage, as well as the acceptance criteria for a project to move from one stage to another. It also describes the Annual Review Process through which those changes will be evaluated and made. 

Project progression \- movement from one stage to another \- allows projects to participate at the level that is most appropriate for them, given where they are in their lifecycle. Regardless of stage, all AAIF projects benefit from a deepened alignment with existing projects and access to mentorship, support, and foundation resources.

Capitalized terms not otherwise defined in this Project Lifecycle Policy have the meanings ascribed to them in the Charter of the AAIF.

---

## Project Proposal Process Overview

### Introduction

This policy sets forth the proposal process for projects to be accepted into the AAIF. The process is the same for both existing projects seeking to move into the AAIF and for new projects to be formed within the AAIF.

### Project Proposal Requirements

Projects must be submitted for contribution to the AAIF through the AAIF [project proposals GitHub repo](https://github.com/aaif/project-proposals). Project submissions must provide the following information:

* name of the project  
* project description (what it does, why it is valuable, origin, and history)  
* statement on alignment with the AAIF mission  
* statement of how the project relates to existing AAIF projects   
* example use cases and evidence of adoption  
* sponsor from the Technical Committee, if identified (a sponsor helps mentor projects)  
* name of the OSI-approved permissive license under which the project is released   
* location of the public repository  
* automated validation and delivery / release processes (public-facing)  
* release methodology and mechanics  
* public-facing contribution process for specifications    
* publicly accessible issue tracker   
* external project dependencies (including licenses of those projects)  
* names of project core maintainers, if different from those submitting proposal  
* description of the project's leadership team and decision-making process  
* documented governance practices (i.e. GOVERNANCE.md), if any  
* list of project's official communication channels (Discord, Slack, mailing lists), if any  
* link to project's website   
* links to social media accounts, if any  
* details of existing financial sponsorship, if any  
* infrastructure needs or requests 

 
Projects can optionally provide the following:

* details of integrations with other AAIF projects  
* a published roadmap  
* openSSF best practices badge  
* desired stage, Sandbox, Growth, or Impact

Projects will be required to: (1) have their existing project host transfer project trademarks and other project assets to the LF as a requirement to join the AAIF; and (2) adopt a technical charter, in the form provided by the LF or as approved by the LF, that specifies the intellectual property policy for the project and how decisions will be made. 

### Project Acceptance Process

The detailed project proposal and acceptance process is presented in [project_proposal_process.md](https://github.com/aaif/technical-committee/blob/main/project_proposal_process.md).

---

## Stages: Definitions and Expectations

Every AAIF project has an associated lifecycle stage. Proposed projects should state their preferred lifecycle stage. AAIF has Sandbox, Growth, Impact, and Emeritus lifecycle stages and new projects may enter the AAIF as Sandbox, Growth, or Impact based on meeting each stage’s requirements.

## Sandbox Stage

### Definition

The Sandbox Stage is the entry point for early-stage projects that are technically viable but do not yet meet the Growth Stage's adoption and community bars. Sandbox lets the AAIF establish neutral governance early, before adoption patterns settle, without committing significant foundation resources. Sandbox status is not an endorsement, and every Sandbox project's README must state this explicitly.

### Examples

1. Protocols or reference implementations whose relevant adoption signal is whether others implement against them, before production patterns exist.
2. Developer tools with strong early interest but not yet documented enterprise production adoption.
3. Infrastructure or framework projects maintained by a credible team, where early neutral governance is more valuable than waiting for scale.

### Expectations

Sandbox projects receive standard infrastructure only (e.g. CI and access to enterprise infrastructure). They are not eligible for mentorship, funding, marketing, or security scanning at this stage. A TC sponsor conducts a checkpoint at six months. Projects are expected to apply for Growth within twelve months; otherwise the Technical Committee opens an Emeritus/archival discussion. Archival from Sandbox is a normal and healthy outcome, not a failure.

### Acceptance Criteria

To be considered for Sandbox Stage, the project must satisfy the following criteria:

* Released under an OSI-approved permissive license.
* Have a working implementation.
* Have at least one actively committing maintainer, with documented intent to grow the contributor base.
* Provide a short written thesis (1-2 pages) covering who would use the project, what would justify Growth graduation, and either documented early external interest or a credible argument for why the project matters pre-adoption.
* Meet the standard AAIF requirements: transfer of project trademarks and other assets to the LF, and adoption of the LF technical charter.
* Receive an absolute majority vote (\>50%) of the Technical Committee.
* Governing Board approval is not required for Sandbox.

### Graduation to Growth

To graduate from Sandbox to Growth, a project must meet the Growth Stage acceptance criteria. In particular:

* Adoption: documented production use by at least two unaffiliated organizations.
* Community: commits from at least two organizations over the prior six months, named committers, and a documented committer-acceptance process.
* Plan: a written growth plan accepted by a TC sponsor, including the project's own definition of Impact graduation.

Graduation follows the standard process: an absolute majority vote (\>50%) of the Technical Committee, subject to final approval of the Governing Board.

## Growth Stage

### Definition

The Growth Stage is for projects that are interested in reaching the Impact Stage, and have identified a growth plan for doing so. Growth Stage projects will receive mentorship from the Technical Committee and are expected to actively develop their community of contributors, governance, project documentation, and other variables identified in the growth plan that factor into broad success and adoption.

In order to support their active development, projects in the Growth stage are eligible to receive access to foundation resources, as approved by the Governing Board. A project's progress toward its growth plan goals will be reviewed on a quarterly basis, and the Technical Committee may decide to move a project to a different stage. 

### Examples

1. Fast adopted projects that are on their way or very likely to become Impact projects.  
2. Projects that are on their way to becoming critical for AI infrastructure and projects.  
3. Projects that need more active support from the Foundation or Technical Committee mentorship in order to reach their goals. 

### Expectations

Projects in the Growth stage are generally expected to exit the Growth stage within two years. It will be the decision of the TC on whether to extend the project in the Growth stage during the annual review process or transition it to the Emeritus stage subject to Governing Board approval. 

### Acceptance Criteria

To be considered for Growth Stage, the project must satisfy the following criteria:

* Technical Committee sponsor to champion the project and provide mentorship.  
* Presentation of a growth plan to demonstrate diverse maintainership, to be done in conjunction with their project mentor(s) at the Technical Committee.  
* Document production use by at least two unaffiliated organizations, with a credible plan to broaden adoption. The Technical Committee retains judgment on quality and scope relative to the AAIF’s mission.  
* Demonstrate an appropriate ongoing flow of commits and merged contributions.  
* Demonstrate that the current level of community participation is sufficient to meet the goals outlined in the growth plan.  
* Receive an absolute majority vote (\>50%) of the Technical Committee to be admitted to Growth Stage, subject to final approval of the Governing Board.

Since these metrics can vary significantly depending on a project's type, scope, and size, the Technical Committee has final judgment on the level of activity that is adequate to meet these criteria.

### Graduation to Impact

To graduate from Growth to Impact, a project must meet the Impact Stage acceptance criteria, and specifially that it has met the goals set out in its growth plan, and is operating self-sufficiently enough that a new growth plan is not required at Impact.

Graduation follows the standard process: an absolute majority vote (>50%) of the Technical Committee, subject to final approval of the Governing Board.

## Impact Stage

### Definition

The Impact Stage is for top-level projects that have reached their growth goals and adoption and are now on a sustaining cycle of development, maintenance, and long-term support. Impact Stage projects have demonstrated wide-scale impact and substantial production deployments. Impact projects have highly active, large, well-established communities and broad industry support.     

### Examples

1. Projects that have publicly documented roadmaps, regular release cycles and plans for Long Term Support ("LTS").  
2. Projects that have themselves become platforms or dependencies for other projects and become critical parts of AI infrastructure or widely adopted AI projects  
3. Projects that are able to attract a healthy number of committers on the basis of their production usefulness (not simply 'developer popularity').  
4. Projects that have many high-profile or well-known end-user implementations.

### Expectations

Impact Stage projects are expected to participate actively in Technical Committee proceedings and provide quarterly project updates, as well as present their roadmaps. They are eligible to receive ongoing AAIF financial support which may include CI infrastructure costs, contractors for documentation, security audits and event travel costs, as well as event participation, and marketing resources.

### Acceptance Criteria

To graduate from Growth status, or for a new project to join as an Impact project, a project must meet the Growth stage criteria plus:

* Have demonstrated significant industry adoption and market impact.  
* Have shown alignment with open principles and displayed project durability.  
* Have a diverse group of maintainers, with multiple organizations represented on the project's governing body.   
* Have a documented and publicly accessible description of the project’s roadmap and release processes.  
* Have a healthy number of committers from at least two organizations. A committer is defined as someone with the commit bit; i.e., someone who can accept contributions to some or all of the project.  
* Explicitly define a process to make changes to the project’s governance, committer acceptance process and a means by which one may become a core maintainer. This is preferably laid out in a GOVERNANCE.md file and references a CONTRIBUTING.md and OWNERS.md file showing the current and emeritus committers.  
* If the project is a Growth project, then other metrics as defined by the applying Project during the application process.  
* For projects entering as an Impact stage project, a growth plan is not required.  
* Receive an absolute majority vote (\>50%) of the Technical Committee to be admitted to Impact Stage, subject to final approval of the Governing Board.

## Emeritus Stage

### Definition

Emeritus projects are projects which the TC or maintainers feel have reached end-of-life. Emeritus projects no longer meet the criteria for a Growth or Impact projects, for instance they may have few or no recent releases, few or no commits, the community may have left the project, core maintainers may have left or the project may have been abandoned entirely.  

### Examples

1. Projects that are are no longer maintained.  
2. Projects that do not plan to release major versions in the future.

### Expectations

Projects in this stage are have little to no activity. Their maintainers may infrequently monitor their repositories and may only push updates to address security issues, if at all. Emeritus projects should clearly state their status in their repo’s README.md and what users or contributors can expect regarding response times or support. If there is an alternative project the maintainers recommend, it should be listed as well. The foundation will continue to hold the IP and any trademarks and domains, but the project does not draw on foundation resources. 

### Acceptance Criteria

Projects may be transitioned to Emeritus status via an absolute majority vote (\>50%) from the Technical Committee or with approval from the Governing Board.

---

## Annual Review Process

The Technical Committee shall conduct an annual review of each project to confirm that its current lifecycle stage remains appropriate and that the project is in good health and making reasonable progress toward its stated goals. Each project shall provide a short written update addressing its maintainership, community activity, release cadence, security posture, and progress against key objectives. Based on this review, the Technical Committee may determine that the project remains in its current stage, recommend corrective actions, or recommend that the project be considered for transition to a different lifecycle stage.  

---

This process is maintained by the AAIF Technical Committee (TC).
