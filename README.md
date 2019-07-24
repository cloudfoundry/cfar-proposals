# cfar-proposals
This is a repository for Cloud Foundry Application Runtime proposals. The purpose of the repository is to provide a way for community members to easily find application runtime proposals and their latest progress. We will be using GitHub Issues to help track proposal lifecycles. We intend to use labels to help with filtering of proposals. Each issue will contain a default parent label in addition to a status and team label.


* **Parent label:** cfar-proposal (all issues have by it default from issue template)
* **Status label:**
  * drafting - Document in drafting state; not ready for review
  * in-review - Under discussion within the community
  * planned - Consensus reached across involved teams
  * in-progress - Implementation in progress
  * complete - Implementation done
  * obsolete - Proposal abandoned
* **Team label:** cli, capi, services api, bits-service, uaa, perm, garden, eirini, garden-windows, diego, persi, networking, haproxy, loggregator, infra, relint, postgres, mysql (to be added by proposal author at the time of issue creation)

Please open one issue per proposal and make sure that issue is in **CFAR Proposal Project**. Issue should only be closed when **implementation is complete** or when proposal has been deemed **obsolete**. For status of all proposals and sample proposal, please see [CFAR Project Board](https://github.com/chenl23/cfar-proposals/projects/1).

---
**Proposal Workflow**
* Open an issue for a new proposal
* Select custom template "Runtime proposal"
  * Update issue with content
  * Add status label
  * Add labels for teams which have a dependency on the proposal
  
**IMPORTANT**
  * **Select Projects “CFAR Proposals”. We need to be in the right project in order for the CFAR Project Board to automatically pick up issues created.**
  * Newly opened issue will be placed in **"In Progress"** cloumn in the CFAR Project Board 
* As proposal cycles through the different possible phases, please update status label to accurately reflect the current progress.

**CFAR Project Board Workflow**
* In Progress = Newly added issue will show up here
* Done = Closed issue will show up here
