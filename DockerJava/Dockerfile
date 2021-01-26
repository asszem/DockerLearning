FROM alpine:latest
USER root

COPY /src /src
WORKDIR /src

RUN apk update
RUN apk fetch openjdk8
RUN apk add openjdk8
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
ENV PATH="$JAVA_HOME/bin:${PATH}"

RUN java -version
RUN javac -version
RUN javac Main.java
CMD ["java", "Main"]
