pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/denoslab/ensf400-lab9-jenkins.git'
            }
        }

        stage('Build') {
            steps {
                sh 'make'
            }
        }

        stage('Test') {
            steps {
                sh './run_tests.sh'
            }
        }
    }
}
