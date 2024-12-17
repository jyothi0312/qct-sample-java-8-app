pipeline {
    agent any

    stages {
        stage('GIT checkout') {
            steps {
                git url: "https://github.com/buddy-works/simple-java-project.git"
                       }
        }
        stage('compile and build') {
            steps {
                echo "MAVEN"
                       }
        }
        stage('CODE quality check') {
            steps {
                echo "sonar code quality"
                       }
        }
        stage('upload artifact(zip , jar) to NEXUS') {
            steps {
                echo "nexus upload"
                       }
        }
        stage('Deploy to production') {
            steps {
                echo "Ansible"
                       }
        }
    }
}
