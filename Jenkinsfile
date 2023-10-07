pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
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
                // Place the appropriate deployment steps here
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
