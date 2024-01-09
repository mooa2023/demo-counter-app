pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', credentialsId: 'Git-Cred', url: 'https://github.com/mooa2023/demo-counter-app.git'
                }
            }
        }
    } 
}
