FROM gradle

WORKDIR /fe-app

COPY /build/libs/frontend-orchestrator-0.0.1-SNAPSHOT.jar /fe-app/lib/frontend-orchestrator-0.0.1-SNAPSHOT.jar

EXPOSE 8081

VOLUME [ "/fe-app/lib" ]

CMD ["java", "-jar", "/fe-app/lib/frontend-orchestrator-0.0.1-SNAPSHOT.jar"]

