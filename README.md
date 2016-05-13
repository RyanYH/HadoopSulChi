# HadoopSulChi
하둡</br>
sudo apt-get update</br>
sudo apt-get install openjdk-7-jdk</br>

usr/lib/jvm/java-7-openjdk-amd64 :path</br>
source environment</br>
R버전 업데이트 3번째</br>

java -version</br>
sudo apt-get install r-base</br>
압축풀고</br>
cd 다운로드</br>
sudo mv ./sts-bundle/ /usr/local</br>
sudo mv ./mongodb /usr/local</br>


cat id_rsa.pub>>authorized_keys</br>
more authorized_keys</br>

cd /home/hadoop/hdfs</br>
ls -al</br>
sudo rm -rf *</br>
ls -al</br>
mkdir name</br>
mkdir data</br>
mkdir mapred</br>
mkdir temp</br>
ls -al</br>
sudo chown sist.root data</br>
sudo chown sist.root name</br>
sudo chown sist.root mapred</br>
sudo chown sist.root temp</br>

--etc안에 environment파일
usr-local-hadoop-hadoop-env java path고치고</br>
core-site namenode -> localhost</br>
mapred-site namenode -> localhost</br>
masters -> localhost</br>
slaves -> localhost</br>

hadoop namenode -format</br>
start-all.sh</br>
jps</br>
   - 해당 노드가 나오지 않으면 폴더 생성x 후에 start-all.sh
   - Datanode
   - Namenode
   - SecondaryNameNode
   - TaskTracker
   - JobTracker
stop-all.sh</br>


localhost:50070</br>
localhost:50030</br>

cd /usr/local/mongodb/bin</br>
mongo</br></br>
sudo apt-get install mongodb-clients</br>
몽고디비 폴더에 data 폴더 생성후 </br>
mongod --dbpath /usr/local/mongodb/data</br>
sudo apt-get install mongodb-server</br>

use mydb</br>
 db.member.insert({no:1,name:"hong",sex:"man"})</br>
db.member.find()</br>
빠져나갈땐 exit</br>

cafe - a-c강의장 POM down</br>
tomcat.apache.org 접속 tomcat8.0 down</br>

cd 다운로드</br>
sudo mv ./apache-tomcat-8.0.33 /usr/local</br>

이클립스에서 </br>
window preference</br>
general keys content ctrl+space</br>
server tomcat 설치</br>
pom 3.1.1 -> 4.2.5</br>
ctrl+f 4.1.6 -> 4.2.5 replacAll </br>

mvnrepository.com</br>
hadoop-core검색</br>
1.2.1 </br>
카페에서 다
ojdbc14 검색</br>

퀀텀db다운 압축풀고 plugins 안에 있는거 이름 맞춰서 복사</br>

퀀텀디비 추가 </br>

terminal</br>
sudo apt-get install r-cran-rjava</br>
sudo apt-get install liblzma-dev</br>
sudo R CMD javareconf</br>

R</br>
library(rJava)</br>
install.packages("Rserve")</br>
usa(ks) choicel</br>

library(Rserve)</br>
Rserve()</br>

q() --> 나가는거</br>

폴더 새문서 data word 생성</br>

다시 터미널</br>
hadoop fs -copyFromLocal /home/sist/word ./word</br>
hadoop fs -ls /user/sist</br>
hadoop fs -cat /user/sist/word</br>

R (사용할떄)</br>
library(rJava)</br>
> library(Rserve)</br>
> Rserve()</br>

hadoop fs -copyFromLocal /home/sist/WordCountProject.jar ./WordCountProject.jar</br>
hadoop fs -ls /user/sist</br>
hadoop jar WordCountProject.jar com.sist.mapred.WordDriver</br>

 hadoop fs -copyToLocal /user/sist/output/part-r-00000 /home/sist/part-r-00000</br>


