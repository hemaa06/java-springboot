pipeline {
    agent any
    stages {
         stage('Test') {
            steps {
                
                sh 'mvn clean package'             
            }
        }
               
        stage('package') {
            steps {
            
                sh 'mvn  clean package -Dsmaven.test.skip=true'
            }
        }
       
        stage('Deploy war') {
            steps {
                echo 'Deploy war'
            }
        }

                    
        }
    
    post {
      failure {
        echo 'Failed'
      }
      success {
        echo 'Success'
      }
    
      }
    }
