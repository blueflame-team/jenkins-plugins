# Jenkins Plugins

How to maintain plugins. 

1. Install Jenkins on your computer with docker

   You can follow most updated instructions on this guide - [Jenkins Github Page](https://github.com/jenkinsci/docker/blob/master/README.md).
   Keep in mind that you need to run a container with a volume in order copy from/to the plugins.
   I installed Jenkins by running the command 
   ```Bash
   docker run -p 8080:8080 -p 50000:50000 --restart=on-failure -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk11
   ```
2. Unzip the plugins.zip file from blueflame-team google drive in your Jenkins container.

3. Restart Jenkins.

4. Now you are able to see all the plugins!
