# base image
FROM ubuntu:18.04

# to update and upgrade 
RUN apt-get update 

# installing mysql
RUN apt-get install -y mysql-server-5.7 python3-mysqldb python3-pip && pip3 install mysqlclient

# copy the shell file into container location
COPY mysql57_start.sh /

# giving the excuting permission for shell file
RUN chmod +x mysql57_start.sh

ENTRYPOINT ["/mysql57_start.sh"]





