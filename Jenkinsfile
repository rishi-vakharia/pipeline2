pipeline {
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git branch: 'main', url: 'https://github.com/rishi2o2o/pipeline2.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x Prog1.py"
                sh "python3 Prog1.py"
            }
        }
        stage('Test Code') {
            steps {
                sh "chmod u+x Test.py"
                sh "python3 Test.py"
            }
        }
    }
}

