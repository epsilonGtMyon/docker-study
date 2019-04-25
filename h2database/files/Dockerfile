FROM adoptopenjdk/openjdk11:latest
EXPOSE 8082
EXPOSE 9082
RUN mkdir /opt/h2-database
ADD http://repo2.maven.org/maven2/com/h2database/h2/1.4.199/h2-1.4.199.jar /opt/h2-database

WORKDIR /opt/h2-database
CMD java -cp h2*.jar org.h2.tools.Server -web -webPort 8082 -webAllowOthers -tcp -tcpPort 9092 -tcpAllowOthers -ifNotExists
