FROM openjdk:11-jre-slim
LABEL maintainer=GJSJ
ENV JAVA_ARGS="-Dfile.encoding=UTF8 -Duser.timezone=GMT+08"
ENV JAR_FILE="user-service.jar"
COPY ./target/${JAR_FILE} ./
EXPOSE 9994
CMD java ${JAVA_ARGS} ${JAVA_OPTS} -jar ${JAR_FILE}