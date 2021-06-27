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

Now if we want to create a script file example script.sh we cant create inside the jenkins server. So we need to exit from jenkins then create .sh file

The command is 
**[vi script.sh]**

Then we can add the script details example
#!/bin/bash
NAME=$1
LASTNAME=$2
echo "Hello $NAME $LASTNAME, How are you doing. Is everything going fine."
.
.

Now we need to copy this script file to jenkins server. The command is

**[docker cp script.sh practical_meninsky:/tmp/script.sh]**

We need to give permission to execute this file for that command
**[chmod +x ./script.sh]**

Now this will save inside the jenkins server.
To see the file inside jenkins sercer the command is 
**[cat /tmp/script.sh]**
To run the script file
**[/tmp/script.sh]**

Docker compose command
**[docker-compose up -d --build]**

Command for genrete ssh key
**[ssh key pairs like ssh-keygen -f remote-key2 -m PEM]**
