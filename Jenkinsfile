pipeline {
    agent any

    tools {
        maven 'mvn-3.8.3'
        jdk 'jdk-11'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -version'
                sh 'java -version'

                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}