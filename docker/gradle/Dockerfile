FROM openjdk:7-jdk

ENV GRADLE_HOME /gradle-2.14
ENV PATH $PATH:$GRADLE_HOME/bin

RUN java -version
RUN echo $JAVA_HOME

ADD https://downloads.gradle.org/distributions/gradle-2.14-bin.zip /gradle-2.14-bin.zip
RUN unzip /gradle-2.14-bin.zip -d / && rm -f /gradle-2.14-bin.zip

RUN gradle -v
