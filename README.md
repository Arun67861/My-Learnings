# My-Learnings


# Jenkins

**Docker**

Docker works like container. Docker can be integrated with Jenkins

First we need to install Docker in our mac.

In the command line tool we need to run the command

Refer this link
https://hub.docker.com/_/jenkins

First command
docker pull jenkins

**Docker Container**

Docker container is the main part in Jenkins with Docker

Command for setuping Docker Container

docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts


