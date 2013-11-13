# Scaling Software Builds with Jenkins

This project provides **Jenkins** setup used for demonstration made during presentation "**Scaling Software Builds with Jenkins**" given at **DevConFu**, *2013* in *Jurmala*, *Latvia* by *Andrey Adamovich*.

## Usage

This setup provides a **Gradle** script (`build.gradle`) that downloads **Jenkins** and all required plugins, 
and copies example job definitions into the **Jenkins** home directory (`jenkins_home`), which is automatically created in the current folder. 

In order to use this script you obviously need to have **JDK** (<http://www.oracle.com/technetwork/java/javase/downloads/index.html>) and **Gradle** (<http://www.gradle.org/>) installed on your machine.
                                                                                                                                              
You can use either `prepare.bat` or `prepare.sh` (depending on your *OS*), or just launch `gradle prepareJenkins` to get all the components fetched from the *Internet* and all directories created.

After that you can use `server.bat` or `server.sh` to launch your local **Jenkins** master. It will take few minutes to initialize and eventually will let you access <http://localhost:1377>.

In order to configure Jenkins EC2 plugin you will need to follow instructions given during presentation: 

![AWS](https://raw.github.com/aestasit/talks2013-devconfu-scaling-builds-setup/master/images/040_JENKINS_EC2_SETTINGS.png)

![AMIs](https://raw.github.com/aestasit/talks2013-devconfu-scaling-builds-setup/master/images/040_JENKINS_EC2_AMI.png)

These instructions as well as some more details are also available in presentation slides: <https://github.com/aestasit/talks2013-devconfu-scaling-builds-slides>.

