# HadoopSulChi
하둡
sudo apt-get update
sudo apt-get install openjdk-7-jdk

usr/lib/jvm/java-7-openjdk-amd64 :path
source environment
R버전 업데이트 3번째

java -version
sudo apt-get install r-base
압축풀고
cd 다운로드
sudo mv ./sts-bundle/ /usr/local
sudo mv ./mongodb /usr/local


cat id_rsa.pub>>authorized_keys
more authorized_keys

cd /home/hadoop/hdfs
ls -al
sudo rm -rf *
ls -al
mkdir name
mkdir data
mkdir mapred
mkdir temp
ls -al
sudo chown sist.root data
sudo chown sist.root name
sudo chown sist.root mapred
sudo chown sist.root temp

usr-local-hadoop-hadoop-env java path고치고
core-site namenode -> localhost
mapred-site namenode -> localhost
masters localhost
slaves localhost

hadoop namenode -format
start-all.sh
jps
stop-all.sh


localhost:50070
localhost:50030

cd /usr/local/mongodb/bin
mongo
sudo apt-get install mongodb-clients
몽고디비 폴더에 data 폴더 생성후 
mongod --dbpath /usr/local/mongodb/data
sudo apt-get install mongodb-server

use mydb
 db.member.insert({no:1,name:"hong",sex:"man"})
db.member.find()
빠져나갈땐 exit

cafe - a-c강의장 POM down
tomcat.apache.org 접속 tomcat8.0 down

cd 다운로드
sudo mv ./apache-tomcat-8.0.33 /usr/local

이클립스에서 
window preference
general keys content ctrl+space
server tomcat 설치
pom 3.1.1 -> 4.2.5
ctrl+f 4.1.6 -> 4.2.5 replacAll 

mvnrepository.com
hadoop-core검색
1.2.1 
카페에서 다
ojdbc 검색
14
퀀텀db다운 압축풀고 plugins 안에 있는거 이름 맞춰서 복사

퀀텀디비 추가 

terminal
sudo apt-get install r-cran-rjava
sudo apt-get install liblzma-dev
sudo R CMD javareconf

R
library(rJava)
install.packages("Rserve")
usa(ks) choicel

library(Rserve)
Rserve()

q() --> 나가는거

폴더 새문서 data word 생성

다시 터미널
hadoop fs -copyFromLocal /home/sist/word ./word
hadoop fs -ls /user/sist
hadoop fs -cat /user/sist/word

R (사용할떄)
library(rJava)
> library(Rserve)
> Rserve()

hadoop fs -copyFromLocal /home/sist/WordCountProject.jar ./WordCountProject.jar
hadoop fs -ls /user/sist
hadoop jar WordCountProject.jar com.sist.mapred.WordDriver

 hadoop fs -copyToLocal /user/sist/output/part-r-00000 /home/sist/part-r-00000


