FROM 10.56.20.3:5000/java:8
VOLUME /tmp
ADD saturn-console-master-SNAPSHOT-exec.jar saturn-console.jar
ENV TZ "Asia/Shanghai"
EXPOSE 9088
CMD ["java", "-DSATURN_CONSOLE_DB_URL=jdbc:mysql://10.1.5.177:3306/saturn_console", "-DSATURN_CONSOLE_DB_USERNAME=saturn", "-DSATURN_CONSOLE_DB_PASSWORD=Ja_6635563", "-Dsaturn.stdout=true", "-Dsaturn.embeddedZk=true", "-jar", "saturn-console.jar"]