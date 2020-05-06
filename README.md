# jenkins_project
## TASK:
#### 1. in this we have to automate the process to deploy the website in production and testing enviroment from github with different             branches(DEV1 AND MASTER) .
#### 2. when quality assurance team what to deploy the same code of testing enviroment to the production enviroment so with the one click         they merge the code.

# ***********
### **To do this task we have to create a 3 different jobs in jenkins** 
### **JOB1:** WHEN DEVELOPER1 PUT ANY CHANGE IN THE DEV1 BRANCH IT AUTOMATICALLY DEPLOY IN THE TESTING ENVIROMET
##        config done in job1:
* ###### 1. with the help of git plugin we mention the repo of the github and the specific branch that jenkins have to monitor each                      minute.
 ######  2. And in the execute shell we write the condational statemnet to launch the container to deploy the testing website and         eveytime the old contaioner which is running is removed and new contain will launch to deploy the website
 ###### 3. with 
                  
