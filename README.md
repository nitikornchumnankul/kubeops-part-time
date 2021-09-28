# KUBEOPS-PART-TIME
## QUSTIONS
- **[NORMAL](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#normal)**
- **[INTERMEDIATE](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#intermediate)**
- **[PROFESSIONAL](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#professional)**
---
### NORMAL

 1. **Describe Git branching strategies ( Git-flow, single branch, feature branch, etc.) which you have used and what purpose does it servers.**
  > **ANSWER:**
   In this question, I have read from [Luis Cuellar](https://www.agileana.com/blog/git-best-practices-for-agile-projects-and-distributed-teams/) who is a blogger on the web page which name is Agileana. I will conclude it on below:

    1.1
    1.2
    1.3 Production
    1.4
    
   **Afterward** I describe about the git-flow which I have used it. followed by:
   1. Git Clone Repository  
   ```git clone https://github.com/username/repository.git```
   2. Create new branch  
   ```git checkout -b new-branch-name```
   3. After I have writed the code to finish, I will do it's on below. Because I'm going to commit that's like save file.   
   ```git add . or git add specific-file.txt```

   4. save file which is edited with message  
    ``` git commit -m "message"```
   5. if new branch name we will set-upstream and push. the command's on below:   
   ```git push --set-upstream origin dev```   
   6. The Main repository ask to pull request.
   7. Compare and Check Source Code.
   8. Comment The Source Code.
   9. Merge pull request to the main branch in this case my own repository. 
##
 2. **How do you revert a commit that has already been pushed and made public?**

 > **ANSWER:**
 
 
##
3. **How do you normally solve conflicts in a feature branch before merge?**
 > **ANSWER:**
##
4.	**“200 OK” what does it mean and show use case this HTTP Status?**
 > **ANSWER:**
##
5.	**“201 Created” what does it mean and show use case this HTTP Status?**
 > **ANSWER:**
##
6. **“301 Moved Permanently” what does it mean and show use case this HTTP Status?6.	“301 Moved Permanently” what does it mean and show use case this HTTP Status?**
 > **ANSWER:**
##
7.	**“400 Bad Request” what does it mean and how to identify the problem?**
 > **ANSWER:**
##
8. **“401 Unauthorized” what does it mean and how to identify the problem?**
> **ANSWER:**
##
9.	**“403 Forbidden” what does it mean and how to identify the problem?**
> **ANSWER:**
##
10.	**“404 Not Found” what does it mean and how to identify the problem?**
> **ANSWER:**
##
11.	**“500 Internal Server Error” what does it mean and how to identify the problem?**
> **ANSWER:**
##
12.	**“502 Bad Gateway” what does it mean and how to identify the problem?**
> **ANSWER:**
##
13.	**“503 Service Unavailable” what does it mean and how to identify the problem?**
> **ANSWER:**
##
14.	**“504 Gateway Timeout” what does it mean and how to identify the problem?14.	“504 Gateway Timeout” what does it mean and how to identify the problem?**
> **ANSWER:**
##
15.	**What are Linux network tools do you use for troubleshooting network problems as well as usage scenarios for each tool?**
> **ANSWER:**

---
### INTERMEDIATE
1.	**Assume we have an application that is designed as below. Our application stopped responding due to an extremely high number of clients in some circumstances.**
-	**We have tried scaling a number of API Gateway and Service A nodes but it didn’t help. What are the possible problems that lies in our system in which components and how to fix them?**   
> **ANSWER:**
##
2.	**How do you keep the docker image smallest as possible?**
> **ANSWER:**
##
3.	**What is the difference between overlay, bridge, host network in Docker? When to use each of them?**
> **ANSWER:**
##
4.	**How does the Kubernetes service talk to each other in the same cluster?
ClusterIP-> kube proxy**
> **ANSWER:**
##
5.	**What’s different between L2, L4, and L7 Load balancers? When to use it?**
> **ANSWER:**

---
## PROFESSIONAL
1.	**Assume that you are using a private cloud for your infrastructure. How do you manage logs, metrics, and alerts for your infrastructure and applications? Which tools do you use and why?
prometeuse**
> **ANSWER:**
##
2.	**How do you secure the following?**
  	- application
  	- infrastructure
  	- data
##
3.	**Base on your experience, how do you reduce your service downtime as much as possible during**
  	- software upgrade
  	- database migration
  	- incident
##
4.	**Configuration management**
    - a. 	Which Among Puppet, chef, Ansible, or another is the best Configuration management tool?
    - b. 	Why?
    - c. 	Do you still need to use it if you already have docker-swarm or Kubernetes?
##
5.	**How do you design your Kubernetes cluster? what DNS, CNI, ingression is being used? Why?**
##
6.	**How do you measure service quality to give the best experience to your customer? (SLO, SLA)**

---