pipeline {
    agent any
    environment {
       VERSION = '1.9.0'
       APP_NAME = 'Example App'
    }
    stages {
        stage('build') {
            steps {
                echo "App name is ${APP_NAME} and version is ${VERSION}"
            }
        }
        stage('test') {
            steps {
                echo "Hi, testing the app...."
            }
        }
    }
}