**List of Proposals 2018**
1. Eirini in 2019 CFAR certification requirements
2. Pluggable Orchestration with Kube backend (“Cube” / “Eirini”)
3. 
***
***
- **Date:** 
- **Owner:** 
- **Work-Group:** 
- **Proposal Name:** 
- **TL;DR Summary:**  
- **Status:** Draft | In Review | Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** 
***
***
- **Date:** 11/16/2018
- **Owner:** Troy Topnik
- **Work-Group:** Erini
- **Proposal Name:** 
- **TL;DR Summary:** So I’d like to propose including Eirini as an alternative CFAR scheduler, assuming it will be passing the relevant tests by the time of certification.
My suggestion is a one line change to the Application Runtime section of the certification requirements:
The Application Runtime portion of a certified offering must include the following components:
[Cloud Controller](https://github.com/cloudfoundry/capi-release/)
[Router](https://github.com/cloudfoundry-incubator/routing-release/)
[Diego](https://github.com/cloudfoundry/diego-release/) or
[Eirini](https://github.com/cloudfoundry-incubator/eirini) 
- **Status:** In Review 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/28180939?p=,,,20,0,0,0::Created,,,20,2,0,28180939,d=5,ct=1&d=5&ct=1)
***
- **Date:** 03/23/2018
- **Owner:** Julz Friedman
- **Work-Group:** Erini
- **Proposal Name:** Pluggable Orchestration with Kube backend (“Cube” / “Eirini”)
- **TL;DR Summary:**  We propose an incubator project to add the ability for CF to use Kubernetes as a scheduler, alongside Diego.
- **Status:** Draft | In Review | Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** In Progress
- **Proposal Link:** [URL](https://docs.google.com/document/d/1qs6UQQDWMkfOpY19XqS3CfvI00jCns876TjplJ6E95s/edit#heading=h.poicq8c1xfqn)
***
- **Date:** 11/0/1/2018
- **Owner:** Stephen Levine
- **Work-Group:** Buildpack 
- **Proposal Name:** Proposal: Sidecars for Cloud Foundry Application Runtime
- **TL;DR Summary:** This proposal[1] suggests a UX for user-specified and buildpack-specified application sidecar processes in CFAR. Each instance of a standalone application process could have any number of associated sidecar process. 
- **Status:** In Progress
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1kC0bywJcTyGYWp0lKt9QkeN-zAgiCCSMyEHGJa-AEig/edit#)
***
- **Date:** 10/31/2018
- **Owner:**  Shubha Anjur Tupil 
- **Work-Group:** Routing
- **Proposal Name:** Cloud Foundry Integration with Istio Pilot and Envoy
- **TL;DR Summary:** Cloud Foundry Routing team will integrate Istio Pilot with Cloud Foundry to enable new features for inbound routing to be delivered using the Envoy proxy, dynamically configured by Istio. We will pursue support for a single multi-tenant deployment of Istio per Cloud Foundry cluster, effectively making it a tightly integrated subsystem of the shared Cloud Foundry management and data planes. 
- **Status:** In Progress 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1LgLY0g39fzpg1_4zTckbH1mOuuSKGvYwp2tkakoe9ys/edit#)
***
- **Date:** 10/19/2018
- **Owner:** Josh Collins
- **Work-Group:** Release Integration
- **Proposal Name:** Proposed Scope for CF-Deployment 6.0
- **TL;DR Summary:**  Scope: 1)Default to cflinuxfs3 2)Overt Windows version selection 3)Update SMB ops files to reference more generic smbbroker 4)Remove all empty/symlinked ops files that were deprecated in previous releases
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1LMr2Ik5T_3lY99I6CBE5_1-hRRixBlDPPqKxh-rARR0/edit#)
***
- **Date:** 09/06/2018
- **Owner:** Josh Collins
- **Work-Group:** Release Integration
- **Proposal Name:** Proposed Scope for CF-Deployment 5.0
- **TL;DR Summary:** Scope: 1)Make Windows 2016 cells default 2)Remove Consul 3)Make Xenial Default 4)Remove log-cache group-reader job 5)Remove all empty/symlinked ops files that were deprecated in previous releases
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1M674BR1gHeKJKJ-lctG-jGDe4oYtRaM0ZGeIfQhB6MQ/edit)
***
- **Date:** 10/05/2018
- **Owner:**  Christopher Brown
- **Work-Group:** CLI
- **Proposal Name:** Handing over the cf-resource and autopilot projects
- **TL;DR Summary:** We (Alex Suraci & Christopher Brown) would like to propose handing the cf-resource and the underlying autopilot CF CLI plugin over to the CF Foundation and the community. The cf-resource is too specialized for the core Concourse distribution and I don’t have time to effectively and responsibly maintain the autopilot plugin anymore.
- **Status:** In Review 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/handing_over_the_cf_resource/26843591?p=,,,20,0,0,0::recentpostdate%2Fsticky,,,20,2,20,26843591)
***
- **Date:** 10/04/2018
- **Owner:** Zach Robinson
- **Work-Group:** CAPI
- **Proposal Name:** Propose removing --no-start from cf push in CLI v7
- **TL;DR Summary:** Propose replace` --no-start` from `cf push` with `cf create-app` in CLI v7	
We’re proposing some changes for the upcoming CF CLI v7 regarding the --no-start flag for the push command. In a previous request for feedback, we learned that the flag is primarily used to get an instance of an app that can have some configuration applied to it prior to running. The proposed change is to maintain that workflow, but in a different way. More details on why changes are necessary are below. Here is the workflow today and the proposed updated workflow.
- **Status:** Planned | In Progress | Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1OPJSUYXMQMtzZmVdnvwI4NiXE0xp4tuLxO3fhhXtGwI/edit)
***
- **Date:** 10/03/2018
- **Owner:** Johannes Tuchscherer 
- **Work-Group:** Loggregator  
- **Proposal Name:** Agent-based Scalable Syslog Draining 
- **TL;DR Summary:** Develop a “shared nothing” architecture which moves the necessary logic of mapping applications to syslog destination into the loggregator agent. Logs flowing through this new system will bypass Loggregator and system entirely. Additionally allowing a configuration for turning off logs through the firehose would take considerable strain off Loggregator in large deployments and allow for less resource consumption. 
- **Status:** Planned | In Progress | Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1ufwv33XEDpSLTjEYDnjQKC3KZ-igVn4WQE3o_SJmtYM/edit#heading=h.s9yu7nl2rwem)
***
