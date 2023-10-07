pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }
    options {
        ansiColor('xterm')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                error 'failed'
            }
        }
    }

    post {
        always {
            echo 'always'
        }
        success {
            echo 'i will run when success'
        }
        failure {
            echo 'i will run when failure'
        }
    }
}
