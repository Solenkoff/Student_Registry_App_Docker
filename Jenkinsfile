pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run security Tests') { 
            steps {
                bat 'npm audit' 
            }
        }
        stage('Run integration Tests') { 
            steps {
                bat 'npm run test' 
            }
        }
    }
}

