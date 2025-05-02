FROM eclipse-temurin:21-jdk-alpine
COPY Main.java .
RUN javac Main.java

FROM eclipse-temurin:21-jre-alpine
WORKDIR /app
COPY --from=0 /usr/src/Main.class .
CMD ["java", "Main"]
# TODO : in next steps (not now)