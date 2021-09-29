![](https://app.travis-ci.com/nitikornchumnankul/kubeops-part-time.svg?branch=mainhttps://app.travis-ci.com/nitikornchumnankul/kubeops-part-time.svg?branch=main)
# KUBEOPS-PART-TIME
## QUSTIONS
- **[NORMAL](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#normal)**
- **[INTERMEDIATE](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#intermediate)**
- **[PROFESSIONAL](https://github.com/nitikornchumnankul/kubeops-part-time/tree/dev#professional)**
---

## NORMAL

 1. Describe Git branching strategies ( Git-flow, single branch, feature branch, etc.) which you have used and what purpose does it servers.
  > **ANSWER:**
   In this question, I have read from [Luis Cuellar](https://www.agileana.com/blog/git-best-practices-for-agile-projects-and-distributed-teams/) who is a blogger on the web page which name is Agileana. I will conclude it on below:

   1.1 Git main branches   
>  **Master:** This branch always reflects a production ready state, and it’s the branch that it’s deployed to the production server.   
>  **Develop:** This branch is used for development and integration of changes.
  
   1.2 Git supporting branches  
> **Feature branches:**  These branches are created from the develop branch, and are utilized to develop new features.  
> **Release branches:**  These are created from the develop branch when the Agile team agrees that the code is stable and is ready to be released to production.  
> **Hotfix branches:**  These are created from the master branch, and are used when changes on develop are not release-ready and a fix to production is required that cannot wait until the upcoming release is stable

   1.3 Git branching and merging  
> **Feature branches:**  
 - Branch off from develop
 - Merge back into develop.
> **Release branches:**  
 - Branch off from develop.
 - Merge back into develop AND master. 
> **Hotfix branches:**  
 - Branch off from master.
 - Merge back into develop AND master.
    
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
   7. Compare and Check Source Code, I saw on the github page which page name is pull request.
   8. Comment The Source Code, . 
   9.  Merge pull request to the main branch in this case my own repository. 
##
 2. **How do you revert a commit that has already been pushed and made public?**

 > **ANSWER:** On this my case I have revert on the public repository. My provider store the source code is Github.
1. I'm going to the public repository, It is changed from anyone. 
2. I'm going to the pull request, The branch is changed. and I'm going to click the revert button on the pull requst of the branch, I will revert it. 
3. The Github, It will generate the new branch which name is revert-2-dev (revert-2-$(branch name)).
4. On my local computer, I will pull the new branch which is reverted. Its name is revert-2-dev.   
   `git branch --set-upstream-to=origin/revert-2-dev revert-2-dev` And `git pull`  
 **On this Case:** we will see conflicts on the revert-2-dev branch.
##
3. **How do you normally solve conflicts in a feature branch before merge?**
 > **ANSWER: On this case I am usually solve manual becuase I will make sure whether It's not show any problem before I commit again. My solution on below:**
1. Check the source code which is changed.   
   `git diff`
2. Delete and Edit the line of source code, It was conflicts.
3. After I finish, I will write command `git add .` and `git commit -m "message"`
4. Checkout to development branch or main branch                  
    `git checkout main | git checkout development` and `git merge feature --no-ff`
##
4.	**“200 OK” what does it mean and show use case this HTTP Status?**
 > **ANSWER:** The request has succeeded. The meaning of the success depends on the HTTP method: GET, POST, PUT, DELETE, OPTION, TRACE.
##
5.	**“201 Created” what does it mean and show use case this HTTP Status?**
 > **ANSWER:** The request has succeeded and a new resource has been created as a result. This is typically the response sent after POST requests, or some PUT requests.
##
6. **“301 Moved Permanently” what does it mean and show use case this HTTP Status?6.	“301 Moved Permanently” what does it mean and show use case this HTTP Status?**
 > **ANSWER:** The request has more than one possible response. The user-agent or user should choose one of them.
##
7.	**“400 Bad Request” what does it mean and how to identify the problem?**
 > **ANSWER:** The server could not understand the request due to invalid syntax.
##
8. **“401 Unauthorized” what does it mean and how to identify the problem?**
> **ANSWER:** Although the HTTP standard specifies "unauthorized", semantically this response means "unauthenticated". That is, the client must authenticate itself to get the requested response.
##
9.	**“403 Forbidden” what does it mean and how to identify the problem?**
> **ANSWER:** The client does not have access rights to the content; that is, it is unauthorized, so the server is refusing to give the requested resource. Unlike 401, the client's identity is known to the server.
##
10.	**“404 Not Found” what does it mean and how to identify the problem?**
> **ANSWER:** The server can not find the requested resource. In the browser, this means the URL is not recognized. In an API, this can also mean that the endpoint is valid but the resource itself does not exist. Servers may also send this response instead of 403 to hide the existence of a resource from an unauthorized client. This response code is probably the most famous one due to its frequent occurrence on the web.
##
11.	**“500 Internal Server Error” what does it mean and how to identify the problem?**
> **ANSWER:** The server has encountered a situation it doesn't know how to handle.
##
12.	**“502 Bad Gateway” what does it mean and how to identify the problem?**
> **ANSWER:** This error response means that the server, while working as a gateway to get a response needed to handle the request, got an invalid response.
##
13.	**“503 Service Unavailable” what does it mean and how to identify the problem?**
> **ANSWER:** The server is not ready to handle the request. Common causes are a server that is down for maintenance or that is overloaded. Note that together with this response, a user-friendly page explaining the problem should be sent. This response should be used for temporary conditions and the Retry-After: HTTP header should, if possible, contain the estimated time before the recovery of the service. The webmaster must also take care about the caching-related headers that are sent along with this response, as these temporary condition responses should usually not be cached.
##
14.	**“504 Gateway Timeout” what does it mean and how to identify the problem?14.	“504 Gateway Timeout” what does it mean and how to identify the problem?**
> **ANSWER:** This error response is given when the server is acting as a gateway and cannot get a response in time.
##
15.	**What are Linux network tools do you use for troubleshooting network problems as well as usage scenarios for each tool?**
> **ANSWER:** I'm usually use ss command and nmap tool

---
### INTERMEDIATE
1.	**Assume we have an application that is designed as below. Our application stopped responding due to an extremely high number of clients in some circumstances.**
-	**We have tried scaling a number of API Gateway and Service A nodes but it didn’t help. What are the possible problems that lies in our system in which components and how to fix them?**   
> **ANSWER:**
##
2.	**How do you keep the docker image smallest as possible?**
> **ANSWER:** It's possible. The docker company have the solution to keep image smallest that call multi-stage builds.
##
3.	**What is the difference between overlay, bridge, host network in Docker? When to use each of them?**
> **ANSWER:** type network of docker that is depend on each case.
> 1. overlay network: That is used when docker network call across server or vm. In this case we may use the docker swarm to control vm or not use depend on the usecase.
> 2. bridge network: private internal network created by docker on the host all containers and we will get internal ip by default. The bridge network is used when container A communicate container B on private network.
> 3. host network: The docker network will use the ip same vm or server which it leaves on.
##
4.	**How does the Kubernetes service talk to each other in the same cluster?
ClusterIP-> kube proxy**
> **ANSWER:**  Type ClusterIP of Kubernete service,The ClusterIP call directly to kube-proxy.
##
5.	**What’s different between L2, L4, and L7 Load balancers? When to use it?**
> **ANSWER:** [L4/L7](https://dev.to/aurelievache/understanding-network-things-part-1-l4-l7-layers-j47)

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
