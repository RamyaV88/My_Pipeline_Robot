pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/KetkiAshtankar/RobotFrameWork.git'
            }
        }
        stage('Install Requirements') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'robot Tests/'
            }
        }
    }
}
