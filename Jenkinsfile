pipeline {     
    agent any      
    stages { 
        
        stage('Test') {  
            steps { 
              sh("echo test"); 
                sh("echo test"); 
                sh("echo test"); 
                sh("echo test12"); 
                sh("echo test12"); 
                sh("echo suhas"); 
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
