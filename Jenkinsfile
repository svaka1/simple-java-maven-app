pipeline {
    agent any
    environment {
       APP_NAME = 'Example App'
       GITHUB_CREDS = credentials('gitHubCreds')
    }
    parameters {
        choice(name:'VERSION',choices:['1.9.0','1.9.1','1.9.2'],description:'Version of the application')
     
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