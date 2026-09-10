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
                bat 'C:\\Users\\ANCY LAZAR\\AppData\\Local\\Programs\\Python\\Launcher\\py.exe -m pip install -r requirements.txt'
            }
        }

        stage('Run Unit Tests') {
            steps {
                bat 'C:\\Users\\ANCY LAZAR\\AppData\\Local\\Programs\\Python\\Launcher\\py.exe -m pytest'
            }
        }
    }
}