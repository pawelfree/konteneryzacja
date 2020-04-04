FROM jboss/wildfly:8.2.1.Final

ADD ./oracle/module.xml $JBOSS_HOME/modules/system/layers/base/com/oracle/main/module.xml
ADD ./oracle/ojdbc6.jar $JBOSS_HOME/modules/system/layers/base/com/oracle/main/ojdbc6.jar
ADD standalone.xml $JBOSS_HOME/standalone/configuration/standalone.xml

RUN $JBOSS_HOME//bin/add-user.sh admin admin --silent

EXPOSE 8080 9090
