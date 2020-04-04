FROM wnameless/oracle-xe-11g-r2

RUN apt-get update
RUN apt-get install vim -y
RUN apt-get install nmap -y

RUN export NLS_LANG=American_America.AL32UTF8

ADD dbaexp.dmp /tmp/dbaexp.dmp

ADD import.sh /docker-entrypoint-initdb.d/init2.sh

EXPOSE 1521
