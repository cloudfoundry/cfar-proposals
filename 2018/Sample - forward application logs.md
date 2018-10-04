
- **Date:** 10/2/2018
- **Owner:** Johannes Tuchscherer
- **Work-Group:** Loggregator 
- **Proposal Name:** A new approach to forwarding application logs to syslog drains    
- **TL;DR Summary:** the loggregator team has come across a few cases where in a big cf deployment with over 9k application-bound syslog drains the scalable syslog adapter is reaching its scaling limits (pun intended). 
We spent some time rethinking the problem regarding the forwarding of application logs to syslog drains. We came to the conclusion that the forwarding best happens as close to the origin of the logs as possible. To implement that strategy, we want to introduce some process on the diego cell (maybe integrated in the loggregator agent aka metron agent), that will forward each application log line directly to the configured syslog endpoint. 
- **Status:** In Review
- **Last Call for Review Date:** 11/2/2018 
- **Proposal Link:** [URL](https://docs.google.com/document/d/1ufwv33XEDpSLTjEYDnjQKC3KZ-igVn4WQE3o_SJmtYM/edit?usp=sharing)
