# Jenkins Plugins

## How to install Jenkins with plugins

1. Install Jenkins on your computer with docker

   You can follow the most updated instructions on [Jenkins Github Page](https://github.com/jenkinsci/docker/blob/master/README.md).
   Keep in mind that you need to run a container with a volume in order to have a persistent plugins directory.
   For example, I installed Jenkins by running the command 
   ```Bash
   docker run -p 8080:8080 -p 50000:50000 --restart=on-failure -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk11
   ```
2. Download plugins.zip file from blueflame-team google drive and copy it to your volume inside jenkins-home directory.

3. Unzip the  in your Jenkins container by running the command 
   ```Bash
   unzip plugins.zip -d /var/jenkins-home/plugins
   ```
4. Restart Jenkins.

5. Now you are able to see all the plugins!

## How to update plugins / add new plugins

1. Go to <Jenkins Url> &#8594; Manage Jenkins &#8594; Manage plugins &#8594; and update/add the plugins.

2. Restart Jenkins and check everything works fine.


