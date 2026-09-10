pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ancylazar/pipelinejob2.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                 bat 'py -m pip install -r requirements.txt'
            }
        }

        stage('Run Unit Tests') {
            steps {
               bat 'py -m pytest'
            }
        }
    }
}
