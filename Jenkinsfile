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
        stage('--deploy--') {
            steps {
		bat 'C:\Git\pknowldege-my-app\BuildDACPAC.bat'
            }
        }
    }
}
