pipeline {
    agent {
        label 'amazon'
    }

    stages {
        stage('get information') {
            steps {
                sh 'pwd'
                sh 'ls'
            }
        }
        stage('molecula test') {
            steps {
                sh 'molecule test'
            }
        }
    }
}
