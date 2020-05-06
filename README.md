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
                  
### **JOB2:**  WHEN MASTER PUT ANY CHANGE IN THE MASTER BRANCH IT AUTOMATICALLY DEPLOY IT IN THE PRODUCTION ENVIROMENT
##        config done in job2:
###### 1. with the help of git plugin we mention the repo of the github and the specific master branch that jenkins have to monitor each                      minute.
######  2. And in the execute shell we write the condational statemnet to launch the container to deploy the website in the production enviroment

###### 3. with the help of **POLLSCM** it moniters the master branch every minute and trigger the job automitaclly when it see any chang
**note: we create a public ip with the help of tunnel and client acn access the site with the help of public ip** 

### **JOB3:**  WHEN QUALITY ASSURANCE TEAM CHECK THAT EVERYTHING IS PERFECT IN TESTING ENVIROMENT THEN THEY MERGE THE DEV1 BRANCH WITH MASTER BRANCH.
##        config done in job3:
###### 1. with the help of git plugin we mention the repo of the github and the specific dev1 branch. 

######  2. In the git plugin we set addational feature **MERGE BEFORE BUILD** in this we mwntion that branch we want to merge with so we want to merge dev1 branch to master branch.

###### 3. and we have to set the credantials and set our github userid and password in the config of jenkins job3 so the job can easely perform the merging task 

**note: we create a public ip with the help of tunnel and client can access the site with the help of public ip**

# TEST VIDEO DRIVE LINKL:
###  https://drive.google.com/open?id=1s9izgh504SF4qPSrLTlWegJtX_aqdj5S

