# My-Learnings


# Jenkins

**Docker**

Docker works like container. Docker can be integrated with Jenkins

First we need to install Docker in our mac.

In the command line tool we need to run the command

Refer this link
https://hub.docker.com/_/jenkins

First command
**[docker pull jenkins]**

**Docker Container**

Docker container is the main part in Jenkins with Docker

Command for setuping Docker Container

**[docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts]**

Now to see the list of active containers 

**[docker ps]**

Now to switch the jenkins folder command

**[docker exec -ti dockerName bash]**

Now for example you created a new project in jenkins and now you enabled the shell scrip
In the shell scrpt you adde a script to redirect some text to temo forder

That is shell scrip
echo "This text you can view in the temp foler" > \tmp\info

Now command to execute this is 

**[cat /tmp/info]**

Now if you want to remove this then use this command

**[rm -rf /tmp/info]**
