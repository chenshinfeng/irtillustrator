# irtillustrator

A java application for illustrating various functionins in item response theory. The interface uses JavaFX. It currently plots binary item response models. Polytomous models will soon be added. Some of the funcitonality still needs tweaking. Hope to have it fully funcitonal by December.  

Building (Updated: 2022-11-03)
========  
Here are the steps for how to build irtillustrator 2017.1 successfully.  

First you need to install Maven & JDK 8 (choose Full JDK with JavaFX):  
[https://maven.apache.org/install.html](https://maven.apache.org/install.html)  
[https://bell-sw.com/pages/downloads/#downloads](https://bell-sw.com/pages/downloads/#downloads) (choose Full JDK with JavaFX)

Open your terminal, build a directory then cd into it, enter the commands below:

git clone https://github.com/chenshinfeng/irtillustrator.git  
git clone https://github.com/chenshinfeng/psychometrics.git

cd psychometrics  
git checkout 50d2167  
mvn clean install -Dfile.encoding=UTF-8 -Dproject.build.sourceEncoding=UTF-8

cd ../irtillustrator  
mvn clean package -Dfile.encoding=UTF-8 -Dproject.build.sourceEncoding=UTF-8

Run:  
java -jar target/irtillustrator-1.0-SNAPSHOT-jar-with-dependencies.jar
