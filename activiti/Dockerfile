FROM marsbard/tomcat

RUN wget -O /tmp/activiti.zip https://github.com/Activiti/Activiti/releases/download/5.19.0.2/activiti-5.19.0.2.zip && \
    unzip /tmp/activiti.zip && ls -al /tmp/

RUN mkdir -p /tomcat/shared/lib
RUN cp /activiti-5.19.0.2/libs/*.jar /tomcat/shared/lib
RUN cp /activiti-5.19.0.2/wars/*.war /tomcat/webapps
