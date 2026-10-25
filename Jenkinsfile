
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/RANI6412/pipelinecicd.git'
            }
        }

        stage('Run Python') {
            steps {
                bat 'py arthtest.py'
            }
        }
    }

    post {
        success {
            echo 'Python pipeline completed successfully!'
        }
    }
}
