<h1>CI/CD Pipeline for Java Application</h1>

This repository demonstrates a complete CI/CD pipeline for a Java application using GitHub Actions.
The pipeline automates building, testing, security scanning, and code quality analysis to ensure reliable and secure software delivery.

🧩 <b>Pipeline Overview</b>

The workflow (.github/workflows/cicd.yml) is automatically triggered on every push to the main branch and includes the following stages:

1️⃣ <b>Compile</b>

Checks out the repository

Sets up JDK 17 (Temurin distribution)

Builds the project using Maven

2️⃣ <b>Security Check</b>

Performs a file system scan with Trivy to detect vulnerabilities

Runs Gitleaks to identify potential secrets or credentials in the codebase

3️⃣ <b>Test</b>

Runs unit tests using Maven to ensure code correctness and stability

4️⃣ <b>Build & SonarQube Scan</b>

Builds the final application artifact

Performs static code analysis using SonarQube to evaluate code quality and maintainability

5️⃣ <b>Deploy</b>

Can be extended to deploy the build artifact to AWS, Docker Hub, or any cloud service.

🛠️ <b>Technologies Used</b>

GitHub Actions – CI/CD automation

Maven – Build and dependency management

Java 17 (Temurin) – Application runtime

Trivy – Vulnerability scanning

Gitleaks – Secrets detection

SonarQube – Code quality analysis


📈 <b>Results</b>

Automated testing and security scanning on every commit

Improved code reliability and maintainability

Early detection of vulnerabilities and misconfigurations
