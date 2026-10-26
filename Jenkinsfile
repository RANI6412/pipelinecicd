

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
                bat 'py -3.16 arthtest.py'
            }
        }
    }
}

