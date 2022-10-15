pipeline {
    // where or who
    agent any
    stages{  
    // collection of stages         
        stage('Package'){
            steps{
                sh 'mvn clean package -Dmaven.test.skip.skip=true'
            }
        }
        stage('Deploy war'){
            steps{
                echo 'Deploy'
            }
        }    
    }    
    post{
        failure{
            echo 'Build faild'
        } 
        success{
            echo 'Build success'
        }   
            
    }      
    
}                                                          