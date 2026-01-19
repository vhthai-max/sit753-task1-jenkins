pipeline {
  agent any
  stages {
    stage('Build') {
      steps { echo 'Build: compile/package using Maven (or Gradle)' }
    }
    stage('Unit and Integration Tests') {
      steps { echo 'Tests: run unit+integration tests using JUnit / NUnit / Jest / Postman/Newman' }
    }
    stage('Code Analysis') {
      steps { echo 'Code Analysis: run static analysis using SonarQube / SonarCloud / ESLint' }
    }
    stage('Security Scan') {
      steps { echo 'Security Scan: scan dependencies/code using npm audit / Snyk / OWASP Dependency-Check' }
    }
    stage('Deploy to Staging') {
      steps { echo 'Deploy to Staging: deploy to AWS EC2 (or Docker staging server)' }
    }
    stage('Integration Tests on Staging') {
      steps { echo 'Staging Tests: run integration tests using Postman/Newman or Selenium' }
    }
    stage('Deploy to Production') {
      steps { echo 'Deploy to Production: deploy to AWS EC2 (or production server)' }
    }
  }
}
