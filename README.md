A template project to create a Docker image for a Java application.
The application exposes an HTTP endpoint.

The Docker build uses a [multi-stage build setup](https://docs.docker.com/develop/develop-images/multistage-build/)
to minimize the size of the generated Docker image.

# Requirements
Docker must be installed. That's it. You do not need a Java JDK or Maven installed.


# Usage

**Step 1:** Create the Docker image according to [Dockerfile](Dockerfile).
This step uses Maven to build, test, and package the [Java application](src/main/java/com/miguno/App.java)
according to [pom.xml](pom.xml).  The resulting image is 87MB in size.
