//Before installing, update the latest version from dlcdn.apache.org 
  tomcat --> version 9 --> see latest version (ex: 9.0.119 ==> then replace all 118 with 119)

//Create vi file and paste in that and run the commands
Ex: vi tomcat.sh
    //paste all commands
Run : sh tomcat.sh


vi tomcat.sh
sh tomcat.sh

sudo apt update -y
sudo apt install openjdk-21-jdk -y
java -version
wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.118/bin/apache-tomcat-9.0.118.tar.gz
tar -zxvf apache-tomcat-9.0.118.tar.gz
sed -i '56  a\<role rolename="manager-gui"/>' apache-tomcat-9.0.118/conf/tomcat-users.xml
sed -i '57  a\<role rolename="manager-script"/>' apache-tomcat-9.0.118/conf/tomcat-users.xml
sed -i '58  a\<user username="tomcat" password="admin@123" roles="manager-gui,manager-script"/>' apache-tomcat-9.0.118/conf/tomcat-users.xml
sed -i '59  a\</tomcat-users>' apache-tomcat-9.0.118/conf/tomcat-users.xml
sed -i '56d' apache-tomcat-9.0.118/conf/tomcat-users.xml
sed -i '21d' apache-tomcat-9.0.118/webapps/manager/META-INF/context.xml
sed -i '22d' apache-tomcat-9.0.118/webapps/manager/META-INF/context.xml
sh apache-tomcat-9.0.118/bin/startup.sh
