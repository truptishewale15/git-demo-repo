pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World from Build'
                sh 'python3 -m py_compile Demo.py'
                sh 'python3 Demo.py'
            }
        }

        stage('Test') {
            steps {
                echo 'Hello World from Test'
                sh 'python3 -m unittest discover -s tests -v'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Hello World from Deploy'
            }
        }
    }
}
