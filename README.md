[![Catacomb Snatch](http://i.imgur.com/uSFJF.png)](https://catacombsnatch.net)

### Links

* [Original source from Mojang](http://assets.mojang.com/mojam/CatacombSnatch_src.zip)
* [Website](http://catacombsnatch.net/)
* [Forum](http://forum.catacombsnatch.net/)
* [Minecraft Forum thread](http://www.minecraftforum.net/topic/1046349-the-catacomb-snatch-project-github)
* [Player & developer wiki](https://github.com/Maescool/Catacomb-Snatch/wiki)
* [Jenkins Build-Bot (Last releases can be found here)](http://ci.catacombsnatch.net/)
* [Download last release](http://ci.catacombsnatch.net/job/Catacomb-Snatch/lastSuccessfulBuild/artifact/build/libs/Catacomb-Snatch-1.1.0-BETA.jar)
* [Download last development build](http://ci.catacombsnatch.net/job/Catacomb-Snatch-Dev/lastSuccessfulBuild/artifact/build/libs/Catacomb-Snatch-1.1.1-SNAPSHOT.jar)
* Chat with the developers on the [Webchat](http://webchat.freenode.net/?channels=catacomb-snatch) or irc.freenode.net #catacomb-snatch
* [libGDX rewrite](https://github.com/Catacomb-Snatch/Catacomb-Snatch)

### How to build project

1. sudo apt-get install openjdk-8-jdk
2. export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
3. echo $JAVA_HOME
4. sudo update-alternatives --config java
5. java -version
	- **should be set to 1.8 version**, output shall be:
	- openjdk version "1.8.0_292"
	- OpenJDK Runtime Environment (build 1.8.0_292-8u292-b10-0ubuntu1~20.04-b10)
	- OpenJDK 64-Bit Server VM (build 25.292-b10, mixed mode)
6. in **build.gradle** update id 'maven' to id 'maven-publish'
7. ./gradlew
8. ./gradlew tasks
9. ./gradlew build
10. ./gradlew run

> When there's a build error, delete .gradle folder in project folder and delete ~/.gradle folder as well and then run ./gradlew again