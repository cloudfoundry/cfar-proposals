**Proposal**

This is a proposal to use GitHub Issues to help track proposal status. We intend to use  labels to help with filtering of proposals. Each issue will contain a default parent label in addition to a status and team label.

* **Parent label:** cfar-proposal (all issues have by it default from issue template)
* **Status label:**
  * drafting - Document in drafting state; not ready for review
  * in-review - Under discussion within the community
  * planned - Consensus reached across involved teams
  * in-progress - Implementation in progress
  * obsolete - Proposal abandoned
* **Team label:** cli, capi, services api, bits-service, uaa, perm, garden, eirini, garden-windows, diego, persi, networking, haproxy, loggregator, infra, relint, postgres, mysql (to be added by proposal author at the time of issue creation)

Please open one issue per proposal and make sure that issue is in **CFAR Proposal Project**. Issue should only be closed when **implementation is complete** or when proposal has been deemed **obsolete**. We recommend as a best practice to add a target milestone. Please see [sample GitHub issue](https://github.com/chenl23/cfar-proposals/issues) for details. For status of all proposals, please [CFAR Project Board](https://github.com/chenl23/cfar-proposals/projects/1).

---
**Workflow**
* Open an issue for a new proposal
* Select custom template "Runtime proposal"
  * Update issue with content
  * Add status label
  * Add labels for teams which have a dependency on the proposal
* **Select Projects “Done in CFAR Proposals”. This is IMPORTANT since we need to be in the right project in order for the CFAR Project Board to automatically pick up issues created.**
* As proposal cycles through the different possible phases, please update status label to accurately reflect the current progress




