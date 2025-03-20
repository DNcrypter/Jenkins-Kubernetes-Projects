
# Jenkins Multi-Stage-Multi-Agent Pipeline for Database, Back-end, and Front-end

# 🍁Introduction
This repository contains a Jenkins pipeline designed to automate the process of verifying the installation of Oracle Database, building a back-end Java application with Maven, and a front-end application with Node.js. It uses Docker containers for each of the stages to ensure a consistent and isolated environment for each part of the process.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
        [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue)](https://www.linkedin.com/in/nikhil--chaudhari/)
        [![Medium](https://img.shields.io/badge/Medium-Writeups-black)](https://medium.com/@nikhil-c)
 

### The pipeline consists of three stages:

* **Oracle Database Check:** Verifies if Oracle Database is available by checking for the sqlplus command.
* **Back-end:** Builds a Java-based back-end application using Maven and JDK 11.
* **Front-end:** Builds a front-end application using Node.js.

In case of a failure in any of the stages, a Slack notification is sent with details of the failure.

# 🍁Prerequisites
Before using this pipeline, ensure you have the following:

### 1. Jenkins Setup:

* Jenkins server running.
* Slack Notification Plugin installed and configured.
* Docker installed on Jenkins agents.

### 2. Slack Setup:

* Slack workspace and channel for notifications.
* Create and configure an incoming webhook for Slack.

### 3. Docker Images:

* `oracle/database:19.3.0-ee` (Oracle Database)
* `maven:3.8.1-adoptopenjdk-11` (Back-end)
* `node:16-alpine` (Front-end)

### 4. Jenkins Plugins:
* Slack Notification Plugin installed and configured in Jenkins.




# Usage
### 1. Clone the repository:

Clone this repository to your local machine or a Jenkins workspace.
```bash
git clone https://github.com/your-username/jenkins-multi-agent-pipeline.git
```
### 2. Create a Jenkins Pipeline Job:

* Go to Jenkins and create a new pipeline job.
* Under Pipeline, select Pipeline script from SCM.
* Choose Git as the SCM and provide the repository URL.
* Jenkins will automatically pull the pipeline script from the repository.


### 3. Run the Pipeline:

* Once the pipeline job is created, you can manually trigger the build or set up a webhook to trigger it automatically.
* The pipeline will run through the stages, and you can check the console output for detailed logs.


### 4. Slack Notifications:

* When the pipeline fails at any stage, a Slack message will be sent to the specified Slack channel with the failure details, including the stage name and the build URL.

# 🍁 Troubleshooting
* **Slack Notifications:** Ensure that your Jenkins Slack configuration is correct, and your webhook is functional. If Slack notifications are not working, check the Jenkins logs for errors related to the Slack plugin.
* **Docker Issues:** If Docker is not running on the Jenkins agents or the images cannot be pulled, ensure that Docker is properly installed and configured on the machine running Jenkins.
* **Pipeline Failures:** If the pipeline fails, check the specific error message in the Jenkins console log for more details. Common errors include missing Docker images or failures during build steps.

# 🍁 Conclusion
We successfully built CICD project, where Jenkins multi-agent pipeline automates building and testing of Oracle, back-end, and front-end applications in isolated Docker environments. It provides seamless integration with Slack notifications for real-time failure alerts.


### Thanks for checking out this project! Happy automation! 🚀

