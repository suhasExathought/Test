pipeline {     
    agent any      
    stages { 
        
        stage('Test') {  
            steps { 
              sh("echo test"); 
                sh("echo test"); 
                sh("echo test"); 
                sh("echo test12"); 
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
