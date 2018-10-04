# Application Runtime Proposals 2018
Please copy below information and start a new entry for your proposal.

Please add incoming proposals at the top of the stack.

- **Date:**
- **Owner:**
- **Work-Group:**
- **Proposal Name:**
- **TL;DR Summary:**
- **Status: In Review | Approved | Obsolete**
- **Last Call for Review Date:**
- **Proposal Link:** 

:new: :new:

## Sample entries START HERE


- **Date:** 10/2/2018
- **Owner:** Johannes Tuchscherer
- **Work-Group:** Loggregator 
- **Proposal Name:** A new approach to forwarding application logs to syslog drains    
- **TL;DR Summary:** the loggregator team has come across a few cases where in a big cf deployment with over 9k application-bound syslog drains the scalable syslog adapter is reaching its scaling limits (pun intended). 
We spent some time rethinking the problem regarding the forwarding of application logs to syslog drains. We came to the conclusion that the forwarding best happens as close to the origin of the logs as possible. To implement that strategy, we want to introduce some process on the diego cell (maybe integrated in the loggregator agent aka metron agent), that will forward each application log line directly to the configured syslog endpoint. 
- **Status:** In Review
- **Last Call for Review Date:** 11/2/2018 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1ufwv33XEDpSLTjEYDnjQKC3KZ-igVn4WQE3o_SJmtYM/edit?usp=sharing)

:new: :new:

- **Date:** 07/25/2018
- **Owner:** Eric Malm
- **Work-Group:** Diego
- **Proposal Name:** Improving Security for HTTP Ingress to CFAR Application Containers
- **TL;DR Summary:** Building on the features and technologies the CF Diego and Routing teams have introduced into the CF App Runtime to improve application routing consistency, security, and stability (https://lists.cloudfoundry.org/g/cf-dev/topic/11900235#7744, which we have often called "route integrity"), the Diego team intends to make it possible for platform operators to opt into improving the security of how traffic ingresses into application containers. In particular, operators would be able to opt into ensuring that only CF system components, or even only the gorouter HTTP routers, would be able to connect to application containers from the infrastructure-provided network.
- **Status:** Approved 
- **Last Call for Review Date:** 09/25/2018
- **Proposal Link:** [URL](https://docs.google.com/document/d/1DjapCLbdgGBmpuWt2P2PV-qm_vUwI_9IZHae9TbN_Pw/edit)


