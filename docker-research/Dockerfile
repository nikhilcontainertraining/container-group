FROM gradle

WORKDIR /be-app

COPY /build/libs/docker-research-0.0.1-SNAPSHOT.jar /be-app/lib/docker-research-0.0.1-SNAPSHOT.jar
#COPY . .

#RUN gradle clean build

#RUN mkdir joke_vol - also works - but is not a container/docker way of doing things

#VOLUME [ "/app/joke_vol" ] - annonymous volumes

VOLUME [ "/be-app/lib" ]

ARG SERVER_NAME=CodingBeast_Build_Args
ENV user_name $SERVER_NAME

#CMD ["gradle", "bootRun"]
CMD ["java", "-jar", "/be-app/lib/docker-research-0.0.1-SNAPSHOT.jar"]
