pipeline {
    //agent { docker { image 'node:6.3' } }
    agent {
        kubernetes {
            containerTemplate {
                name 'node'
                image 'node:6.3'
                ttyEnabled true
            }
        }
    }
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
