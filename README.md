# jenkins_project
## TASK:
#### 1. in this we have to automate the process to deploy the website in production and testing enviroment from github with different             branches(DEV1 AND MASTER) .
#### 2. when quality assurance team what to deploy the same code of testing enviroment to the production enviroment so with the one click         they merge the code.

# ***********
### **To do this task we have to create a 3 different jobs in jenkins** 
### **JOB1:** WHEN DEVELOPER1 PUT ANY CHANGE IN THE DEV1 BRANCH IT AUTOMATICALLY DEPLOY  IT IN THE TESTING ENVIROMET
##        config done in job1:
###### 1. with the help of git plugin we mention the repo of the github and the specific dev1 branch that jenkins have to monitor each                      minute.
######  2. And in the execute shell we write the condational statemnet to launch the container to deploy the testing website and         eveytime the old contaioner which is running is removed and new contain will launch to deploy the website
###### 3. with the help of **POLLSCM** it moniters the dev1 branch every minute and trigger the job automitaclly when it see any change  
                  
## **JOB2:**  WHEN MASTER PUT ANY CHANGE IN THE MASTER BRANCH IT AUTOMATICALLY DEPLOY IT IN THE PRODUCTION ENVIROMENT
##        config done in job2:
###### 1. with the help of git plugin we mention the repo of the github and the specific master branch that jenkins have to monitor each                      minute.
######  2. And in the execute shell we write the condational statemnet to launch the container to deploy the website in the production enviroment

###### 3. with the help of **POLLSCM** it moniters the master branch every minute and trigger the job automitaclly when it see any chang
**note: we create a public ip with the help of tunnel and client acn access the site with the help of public ip** 
