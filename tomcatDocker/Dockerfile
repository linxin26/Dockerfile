FROM         Ubuntu:14.10
MAINTAINER    linx<644299146@qq.com>

#把java与tomcat添加到容器中
ADD jdk-8u31-linux-x64.tar.gz /usr/local/
ADD apache-tomcat-8.0.20.tar.gz /usr/local/

#配置java与tomcat环境变量
ENV JAVA_HOME /usr/local/jdk1.8.0_31
ENV CLASSPATH $JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
ENV CATALINA_HOME /usr/local/apache-tomcat-8.0.20
ENV CATALINA_BASE /usr/local/apache-tomcat-8.0.20
ENV PATH $PATH:$JAVA_HOME/bin:$CATALINA_HOME/lib:$CATALINA_HOME/bin
 
#容器运行时监听的端口
EXPOSE  8080