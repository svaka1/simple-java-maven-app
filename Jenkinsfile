pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat "mvn clean install"
            }
        }
        stage('test') {
            steps {
                echo "Hi, building the app...."
            }
        }
    }
}