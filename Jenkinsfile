pipeline {
    agent any
    stages {
        stage('--START PIPELINE--') {
            steps {
                echo "Begin pipeline execution"
            }
        }
        stage('---clean---') {
            steps {
                bat "mvn clean"
            }
        }
        stage('--test--') {
            steps {
                bat "mvn test"
            }
        }
        stage('--package--') {
            steps {
                bat "mvn package"
            }
        }
        stage('--Deploy dacpac--') {
            steps {
                bat cd /
		bat cd C:\Git\pknowldege-my-app
		bat BuildDACPAC.bat
            }
        }
    }
}
