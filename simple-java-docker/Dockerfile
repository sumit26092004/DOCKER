FROM openjdk:17-jdk-alpine

WORKDIR /app

# Copy Java source into container
COPY src/ ./src/

# Compile Java code into /app/bin
RUN mkdir -p bin && javac -d bin src/*.java

# Run the Main class from bin
CMD ["java", "-cp", "bin", "Main"]
