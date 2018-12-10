**List of Proposals 2018**
- Eirini in 2019 CFAR certification requirements
- Pluggable Orchestration with Kube backend (“Cube” / “Eirini”)
- 
***
TEMPLATE: Please copy and use it for new entries.
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
- **Proposal Name:** Eirini in 2019 CFAR certification requirements
- **TL;DR Summary:** Eirini is coming, and a number of us are keen to see Kubernetes-native app scheduling in CFAR distributions as soon as possible. Ideally we would like these distributions to be certified by the CF Foundation when they are released. We recognize that Eirini is still in incubation, but it’s getting closer to feature parity with Diego every day. The Cloud Foundry acceptance tests (CATs) are almost all passing, and are expected to be fully passing by the time the certification requirements are released, but the 2019 requirements are currently being drafted.So I’d like to propose including Eirini as an alternative CFAR scheduler, assuming it will be passing the relevant tests by the time of certification. My suggestion is a one line change to the Application Runtime section of the certification requirements:
The Application Runtime portion of a certified offering must include the following components:
[Cloud Controller](https://github.com/cloudfoundry/capi-release/)
[Router](https://github.com/cloudfoundry-incubator/routing-release/)
[Diego](https://github.com/cloudfoundry/diego-release/) or
[Eirini](https://github.com/cloudfoundry-incubator/eirini) 
- **Status:** In Review 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/28180939?p=,,,20,0,0,0::Created,,,20,2,0,28180939,d=5,ct=1&d=5&ct=1)
***
- **Date:** 11/01/2018
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
- **Date:** 09/20/2018
- **Owner:** Kartik Lunkad
- **Work-Group:** Garden-Windows
- **Proposal Name:** Ephemeral Disk Support for Windows 1709 and Windows 1803 Stemcells
- **TL;DR Summary:** This feature will allow you to have a much smaller root disk footprint, and allow you to use ephemeral disk for your applications! We have now reduced the root disk to be 30GB.  
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/25835274?p=,,,20,0,0,0::Created,,,20,2,40,25835274,d=5,ct=1&d=5&ct=1)
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
- **Date:** 08/17/2018
- **Owner:**  Josh Collins
- **Work-Group:** Release Integration 
- **Proposal Name:** REQUEST for REVIEW - Proposed Scope for CF-Deployment v4.0
- **TL;DR Summary:** Based on the feedback generated during the cf-deployment v3.0 retro and observations of the impact of 3.0 on the CF development community CI's, I'd like to share and gather feedback on proposed scope of the next major release of cf-deployment. 
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1C8DYPaohFHN8pg1QHQQtgqaZqoGXATSf3ErDaML4FPQ/edit?usp=sharing )
***
- **Date:** 08/03/2018
- **Owner:** Matthias Winzeler
- **Work-Group:** Diego
- **Proposal Name:** Add support for multiple Credhubs to CF/Diego
- **TL;DR Summary:**  Currently, the CF ecosystem supports two deployment architectures of Credhub (https://docs.cloudfoundry.org/credhub/#deployment-architecture ):
Colocated with BOSH, used for the secrets of the BOSH director
Deployed standalone as its own deployment (“Runtime Credhub”), used for the secrets of service brokers, supported by CF for https://github.com/cloudfoundry-incubator/credhub/blob/master/docs/secure-service-credentials.md to interpolate creds.
Currently, Diego only supports one credhub endpoint for the Runtime Credhub (which is injected via CloudController in the 
- **Status:** Draft | In Review | Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/24161998?p=,,,20,0,0,0::Created,,,20,2,80,24161998,d=5,ct=1&d=5&ct=1)
***
- **Date:** 07/25/2018
- **Owner:** Eric Malm
- **Work-Group:** Diego 
- **Proposal Name:** Proposal: Improving Security for HTTP Ingress to CFAR Application Containers
- **TL;DR Summary:**  Building on the features and technologies the CF Diego and Routing teams have introduced into the CF App Runtime to improve application routing consistency, security, and stability (https://lists.cloudfoundry.org/g/cf-dev/topic/11900235#7744, which we have often called "route integrity"), the Diego team intends to make it possible for platform operators to opt into improving the security of how traffic ingresses into application containers. In particular, operators would be able to opt into ensuring that only CF system components, or even only the gorouter HTTP routers, would be able to connect to application containers from the infrastructure-provided network.
- **Status:**  In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1DjapCLbdgGBmpuWt2P2PV-qm_vUwI_9IZHae9TbN_Pw/edit)
***
- **Date:** 07/13/2018
- **Owner:**  Shubha Anjur Tupil
- **Work-Group:** Routing
- **Proposal Name:** roposal for weighted routing user experience in Cloud Foundry
- **TL;DR Summary:**  The CF Routing team has received feedback from many users that support for weighted routing would make it easier to accomplish their goals. This feature will be the first to be delivered using istio-release as the new routing subsystem for CF. The CF Routing team is eager to have this subsystem adopted in order to get feedback from operators. All future routing features, for north-south as well as east-west, will be delivered using istio-release. For details on our plans for Istio in CF, see Cloud Foundry Integration with Istio Pilot and Envoy.
- **Status:** In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1XDkGEe0i2t0UHBcOjJMUJhQ_ksYh-Jes3uOJiOFEqg0/edit#)
***
- **Date:** 07/13/2018
- **Owner:**  Julz Friedman
- **Work-Group:** Garden
- **Proposal Name:** Feature Narrative / Proposal: Let's fix* CPU Sharing and Metrics in CF
- **TL;DR Summary:**  Containers should have a ‘CPU entitlement’ (still proportional to requested memory limit, for now) which is the amount of CPU a container is entitled to average over time. (This is as opposed to the current, opaque, “relative share” cpu sharing).
- **Status:**  In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/16TvBsZSInjy7zoboSQWRJo30lmxr07tvd40_GzpfD3I/edit#heading=h.95wb43g0oq3n)
***
- **Date:** 06/12/2018
- **Owner:** Zac Robinson
- **Work-Group:** CAPI
- **Proposal Name:** Feedback request: Proposed changes to capi-release nfs_server.share_path
- **TL;DR Summary:** Recently on the CAPI team we've been updating our BOSH jobs to run within BPM. BPM is opinionated with regards to which directories can be mounted within its containerized jobs. This means that in order to properly support NFS, we will need to update the default nfs_server.share_path to be located within the "/var/vcap/data" directory on Cloud Controller BOSH instances. 
- **Status:**  Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/22015965?p=,,,20,0,0,0::Created,,,20,2,140,22015965,d=5,ct=1&d=5&ct=1)
***
- **Date:** 04/04/2018
- **Owner:** Zach Brown
- **Work-Group:** Services API
- **Proposal Name:** Proposal for incubation in the Extensions PMC: MS-SQL Service Broker
- **TL;DR Summary:**  This project aims to create an Open Service Broker that automates tasks associated with creating schemas, provisioning users, and providing credentials for applications wishing to make use of SQL Server databases within Cloud Foundry. The MVP broker can be used to interact with an existing (external to Cloud Foundry) SQL Server Database Engine. Via the broker, applications will be able to connect to SQL Server using the standard service broker “bind” semantics.
- **Status:** Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1cUjY2fqdHn8GPjqp4jY-wjGlPIhZMYj4Qv7zeGf_6T8/edit#heading=h.j5ilo486aynh)
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
- **Date:** 03/19/2018
- **Owner:** Adam Hevenor
- **Work-Group:** Loggregator
- **Proposal Name:** A New Packaging Approach - CLI Tools Pushing Apps and the Story about the #loggregator “space drain” experiment
- **TL;DR Summary:**  The Loggregator team has recently been seeing a ton of benefit from developing CLI plugins. Specifically they are quick to develop, and distribute and lend themselves well to rapid iteration based on feedback. Developing our noisy neighbor nozzle we worked closely with the Pivotal early access program to meaningfully shape the final product that we eventually posted here. This feedback loop helped us focus on the trying to solve specific packaging UX problems with a plugin and arrived at a new techniques that packaged apps along with a CLI plugin. We have since taken those ideas a step further.
- **Status:** Draft | In Review | Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/15605285?p=,,,20,0,0,0::Created,,,20,2,200,15605285,d=5,ct=1&d=5&ct=1)
***
- **Date:** 03/13/2018
- **Owner:** Adam Hevenor
- **Work-Group:** Loggregator
- **Proposal Name:** Feature Narrative - Isolated Loggregator Components
- **TL;DR Summary:** One of the benefits we see of having re-engineered the persistance layer of Loggregator (see log-cache announcement) is a simpler architecture which can be deployed to multiple times within Cloud Foundry Application Runtime. This makes the concept of isolation segments one that works nicely with Loggregator, which is a feature we have received consistent feedback on over the last year. 
- **Status:** In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1w_j6pf9v-lobXEfUmOYWKTyCtRLmKsOayVRfS2kZQPs/edit#heading=h.h4kd8w9hjl6t)
***
- **Date:** 03/12/2018
- **Owner:** Shubha Anjur Tupil
- **Work-Group:** Routing
- **Proposal Name:** Feedback request: Disable logging Client IP’s in the Gorouter logs for compliance with the EU General Data Protection Regulation (GDPR)
- **TL;DR Summary:**  In lieu of The EU General Data Protection Regulation (GDPR), the routing team is investigating adding manifest properties to allow an operator to disable logging the client IP's in the X-Forwarded-For header in the access and error logs for Gorouter. Enforcement of The EU General Data Protection Regulation (GDPR) (https://www.eugdpr.org/) begins May 28th and imposes steep fines. This law says that companies will be fined if they are capturing PII. The Gorouter currently captures Client IP addresses that are included in that definition. We are exploring manifest properties to allow operators to disable logging the originating client IP.
- **Status:** In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/14512703?p=,,,20,0,0,0::Created,,,20,2,220,14512703,d=5,ct=1&d=5&ct=1)
***
- **Date:** 03/08/2018
- **Owner:** Matt Cholick
- **Work-Group:** Services API
- **Proposal Name:** Automating Security Groups and Brokered Services
- **TL;DR Summary:**  I proposed an enhancement to let the service broker api to return the service endpoint info as part of the bind call so Cloud Controller or whatever is running the platform can create the ASG or its equivalent to let the app communicate to that endpoint. This lets the service broker be transparent to where its running and what platform or the credentials of the platform while the platform manage the required policy/security handling.
- **Status:** Planned | In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URl](https://lists.cloudfoundry.org/g/cf-dev/topic/14245515?p=,,,20,0,0,0::Created,,,20,2,220,14245515,d=5,ct=1&d=5&ct=1)
***
- **Date:** 03/06/2018
- **Owner:** Eric Malm
- **Work-Group:** Diego
- **Proposal Name:** Proposal: Readability Improvements to Diego Component Logs
- **TL;DR Summary:**  The Diego team is planning to make some modest improvements to the readability of the Diego component logs. Primarily, we'd like to make each log-line's timestamp ISO 8601/RFC 3339 compliant (that is, of the form "2018-03-06T12:34:56.789012345Z") and its log level a human-readable string. 
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1D3GK2IUGQz_3fCuuLPNWz7Yb8eiKKZ9k-78LwNHWtuU/edit#)
***
- **Date:** 02/30/2018
- **Owner:**  Julz Friedman
- **Work-Group:** Garden
- **Proposal Name:** Proposal: Garden support for Containerd
- **TL;DR Summary:** Garden-runc [0] should support delegating to containerd [1] to run containers.
[0]: https://github.com/cloudfoundry/garden-runc-release
[1]: https://github.com/containerd/containerd
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/11hFXFPAz4yHtphYQArmhAqw5nD4KgMVmXRWIrE2D7Ko/edit?usp=sharing)
- **Date:** 02/13/2018
- **Owner:** Michael Rhodes 
- **Work-Group:** Services API
- **Proposal Name:** Open Service Broker API enhancement for generic actions / extensions needs reviews
- **TL;DR Summary:** Any service broker author, service operator or openapi expert that has some free time to look at this proposal and PR please do. 
- **Status:** In Progress 
- **Last Call for Review Date:** 
- **Proposal Link:** {URL)[https://lists.cloudfoundry.org/g/cf-dev/topic/11164454?p=,,,20,0,0,0::Created,,,20,2,260,11164454,d=5,ct=1&d=5&ct=1]
***
- **Date:** 02/09/2018
- **Owner:** Adam Hevenor
- **Work-Group:** Loggregator
- **Proposal Name:** Metric Drains - A New Way for App Developers to Monitor their Containers
- **TL;DR Summary:** In service to our mission of providing all users of Cloud Foundry observability of their systems the Loggregator team is excited to offer a new feature for App Developers to use external monitoring tools for monitoring their applications without the need for FIrehose scope. This is accomplished by the use of User Provided Syslog Drains and a new CLI Plugin and we have called the new feature Metric Drains.  
- **Status:**  In Progress | Complete | Obsolete
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://lists.cloudfoundry.org/g/cf-dev/topic/10766104?p=,,,20,0,0,0::Created,,,20,2,260,10766104,d=5,ct=1&d=5&ct=1)
***
- **Date:** 01/11/2018
- **Owner:** Dies Koper
- **Work-Group:** CLI
- **Proposal Name:** Value Substitution in App Manifest Proposal
- **TL;DR Summary:** The cf CLI team has explored how to better address the problems that the deprecated app manifest inheritance feature intended to solve, as well as providing secrets when pushing apps without storing them with other app configuration in the app manifest. 
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1yax7Hjw_YJiKwh2aAwY3r-BtuDpJvoUaPvQ7B3sTju4/edit#heading=h.ao5mzn496lr6)
***
- **Date:** CAPI
- **Owner:** Dies Koper, Jay Badenhope, Zach Robinson
- **Work-Group:** 
- **Proposal Name:** Proposal for Server Side App Manifest
- **TL;DR Summary:** Moving the processing logic of the app manifest supported by the cf CLI and Java client to a server API. This would make it simpler for manifests to be processed in the same way by cf CLI, Java, and any other clients.
For the cf CLI, `v3-push` would use this API to add support for app manifests with CC V3 features such as multiple buildpacks and processes.
- **Status:** In Progress 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1JBWFP86t5mgu7_Cie97AIDlsFGyHIGsfJb3kmcNtHZE/edit#) 
***
- **Date:** 01/08/2018
- **Owner:** Eric Malm
- **Work-Group:** Diego
- **Proposal Name:** Proposal for breaking changes in Diego v2.0
- **TL;DR Summary:** The Diego team is planning to cut v2.0 of diego-release soon with a set of breaking changes from the v1.x version series. These changes are intended primarily to reduce the complexity of the BOSH properties in the release and the underlying configurations of the Diego components as the release has evolved over the past year. Most of the proposed changes are already present in the cf-deployment manifest, and if you have already migrated to it (which you should do soon!) then we'll be working to ensure that the transition across the major version bump is seamless for you. 
- **Status:** Complete 
- **Last Call for Review Date:** 
- **Proposal Link:** [URL](https://docs.google.com/document/d/19RPbphzK6osx6gA_L-V8Q-ggZD5JpUy3xhkK3KconpU/edit)
***
