pipeline {
    agent any

    tools {
       jdk 'JDK17'
        maven 'maven1'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install -DskipTests'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}

