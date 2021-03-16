pipeline {
    agent any
    environment {
       VERSION = '1.9.0'
       APP_NAME = 'Example App'
       GITHUB_CREDS = credentials('gitHubCreds')
    }
    stages {
        stage('build') {
            steps {
                echo "App name is ${APP_NAME} and version is ${VERSION}"
                echo "Current build is ${BUILD_NUMBER}"
            }
        }
        stage('git-creds') {
            steps {
                echo "Id is ${GITHUB_CREDS_USR} and password is ${GITHUB_CREDS_PSW}"
            }
        }
    }
}