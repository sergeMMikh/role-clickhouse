pipeline {
    agent {
        label 'amazon'
    }

    stages {
        stage('refresh role') {
            steps {
                sh 'pwd'
                dir('role-clickhouse') {
                    sh 'pwd'
                    sh 'git fetch'
                }
            }
        }
        stage('molecula test') {
            steps {
                sh 'pwd'
                dir('role-clickhouse') {
                    sh 'pwd'
                    sh 'molecule test'
                }
            }
        }
    }
}
