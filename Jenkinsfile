pipeline {
    agent {label 'java'}
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

        stage('Sonar analasys') {
            steps {
                echo 'Sonar Qube'
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

    } 
    post {
        failure {
            echo 'failure'
        }
        success{
            echo 'success'
        } 
        abort {
            echo 'abort'
        }
        always { 
            echo 'I will always say Hello again!'
        }
    }
 
}    
                                                          