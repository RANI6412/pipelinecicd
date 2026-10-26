

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
                bat '''
                    set PYTHONHOME=
                    set PYTHONPATH=
                    py --version
                    py -c "import encodings; print('Python is working')"
                    py arthtest.py
                '''
            }
        }
    }
}

