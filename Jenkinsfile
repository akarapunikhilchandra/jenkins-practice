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
        stage('init') {
            steps {
                sh '''
                cd 01-vpc
                ls -ltr
                pwd
                terraform init
                '''
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
