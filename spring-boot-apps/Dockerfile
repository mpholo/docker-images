FROM centos

RUN yum install -y java-11-openjdk-devel



 

VOLUME /tmp

ENV SPRING_PROFILES_ACTIVE postgres

COPY  grocery-web-0.0.1-SNAPSHOT.jar myapp.jar
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/ ./urandom","-jar","/myapp.jar"]
