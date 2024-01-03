## Using SonarQube to Analyze a Java Project

### What is Sonarqube?

SonarQube is an open-source platform for continuous inspection of code quality. Using static code analysis, it tries to detect bugs, code smells and security vulnerabilities. SonarQube supports many languages through built-in rulesets and can also be extended with various plugins.

It is actively developed and well integrated. Many plugins are available to use it as part of continuous integration pipelines, including for Maven, Jenkins and GitHub.

Its built-in rulesets can be extended with plugins that are more security-oriented. For instance, we will use the FindBugs plugin to take advantage of FindBugs rules.

It can also report things such as duplicated code, code coverage or coding standards.

This project was generated with [Docker-compose]([https://github.com/angular/angular-cli](https://docs.docker.com/compose/)) version 3.9.

## Installation

### Prerequisites
Java 8 and above
Maven
Docker

### Installing SonarQube Locally via Docker

To ease things up, here is the Docker Compose YAML file we are going to use:

Clone the repo and stat the container

Please run `docker-compose up -d` to start all the required containers (sonar & DB).

check the docker service running `docker-compose ps`

Shurtdown the sonar and db server `docker-compose down` 



### Sonar server Access
access the sonar server
Once started and you can hit the URL `http://localhost:9000/`
login with defualt credential `admin:admin`

### Running Analysis
First, we need to create a project in the SonarQube.

Let’s give the project display name and the key then click on the setup button.

