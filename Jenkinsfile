pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }

        stage('Sonar Qube') {
            steps {
                echo 'Sonar Qube'
            }
        }

    }
    stage('Push to artifactory') {
            steps {
                echo 'Push to artifactory'
            }
        }
        stage('Deploy to QA') {
            steps {
                echo 'Deploy to QA'
            }
        }
        stage('Deploy to prod') {
            steps {
                echo 'Deploy to prod'
            }
        }
    post {
        Failure {
            echo 'failure'
        }
        sucess{
            echo 'sucess'
        } 
        abort {
            echo 'abort'
        }
        always { 
            echo 'I will always say Hello again!'
        }
    }
}    
                                                           