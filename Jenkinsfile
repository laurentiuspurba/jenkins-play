pipeline {
    /* agent { docker { image 'node:6.3' } } */
    agent {
        docker { image 'node:7-alpine' }
    }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
                sh 'node --version'
            }
        }
    }
    post {
        always {
            echo 'Always runs'
        }
    }
}
