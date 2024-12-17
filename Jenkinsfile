pipeline {
    agent any

    stages {
        stage('GIT checkout') {
            steps {
                git url: "https://github.com/jyothi0312/qct-sample-java-8-app.git"
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
