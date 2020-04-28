pipeline {     
    agent any      
    stages { 
        
        stage('Test') {  
            steps { 
              sh("echo test"); 
            } 
        }         
    }
    post{
        always{
            cleanWs()
            sh "echo Workspace clean up successful"
        }
    } 
} 
