pipeline { 
    // agent { 
    //     docker { 
    //         image 'node:8.15.0' 
    //         args '-p 3000:3000'   
    //     } 
    // } 
    agent any 
    // environment{ 
    //     AWS_ACCESS_KEY_ID='AKIAWHM436GADCW2YFBX' 
    //     AWS_SECRET_ACCESS_KEY='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' 
    //     AWS_DEFAULT_REGION='ap-south-1' 
    //     AWS_LAMBDA_S3BUCKET_NAME='saipetpreforms-lambda-deployment'  
    //     AWS_LAMBDA_OUTPUT_TEMPLATE_FILE='smerp.yaml'
    //     AWS_LAMBDA_INPUT_TEMPLATE_FILE = 'template-dev.yaml'
    //     AWS_LAMBDA_STACK_NAME='SAI-SMERP-DEV'  
    //     AWS_LAMBDA_CAPABILITIES='CAPABILITY_IAM'  
    // } 
    stages { 
        // stage('Build') {  
        //     steps { 
        //         dir("src"){     
        //             sh("echo pulling from branch ... ${env.BRANCH_NAME}"); 
        //             sh("npm install"); 
        //             sh("npx webpack"); 
                     
        //         }  
        //     } 
        // } 
        stage('Test') {  
            steps { 
              sh("echo test"); 
            } 
        } 
        // stage('Deploy') {  
        //     steps { 
        //          dir("src"){ 
        //              sh("echo Deploy Stage!!");  
        //             sh("sam build");  
        //             sh("sam package --s3-bucket ${env.AWS_LAMBDA_S3BUCKET_NAME} --template-file ${env.AWS_LAMBDA_INPUT_TEMPLATE_FILE} --output-template-file ${env.AWS_LAMBDA_OUTPUT_TEMPLATE_FILE}");  
        //             sh("sam deploy --template-file ${env.AWS_LAMBDA_OUTPUT_TEMPLATE_FILE} --stack-name ${env.AWS_LAMBDA_STACK_NAME} --region ${env.AWS_DEFAULT_REGION} --capabilities ${env.AWS_LAMBDA_CAPABILITIES}")  
                   
        //         } 
        //     } 
        // } 
    }
    post{
        always{
            cleanWs()
            sh "echo Workspace clean up successful"
        }
    } 
} 
