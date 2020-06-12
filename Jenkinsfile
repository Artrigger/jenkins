pipeline {
    agent { docker { image 'node:6.3' } }
    // options {
    //     buildDiscarder(logRotator(numToKeepStr: '2'))
    // }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
        stage('test') {
            steps {
                sh 'hostname'
            }
        }
    }
}