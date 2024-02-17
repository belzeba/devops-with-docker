# NOTE: for this the whole material -repository was cloned and then the Dockerfile was created, and used, in
# /home/ari/docker-assignments/devops-with-docker/part1/exercises/exercise_1.11/material-applications/spring-example-project/

# Get OpenJDK 8
FROM openjdk:8-jdk

# Just copy everything in the folder here/inside the ocntainer
COPY . .

# Run maven package cycle
RUN ./mvnw package

# Execute things
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

