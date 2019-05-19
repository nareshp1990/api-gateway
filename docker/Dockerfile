FROM java:8

MAINTAINER patchipulusu.naresh@gamil.com

ADD docker/startup.sh /
RUN mkdir -p /etc/conf/api-gateway/

ADD src/main/resources/logback-spring.xml /etc/conf/api-gateway/logback-spring.xml

EXPOSE 8080
# run the application
#CMD [""]
ENTRYPOINT ["sh", "/startup.sh"]

# add the jar file
ADD target/api-gateway.jar api-gateway.jar