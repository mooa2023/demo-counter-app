pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                git branch: 'main', credentialsId: 'Git-Cred', url: 'https://github.com/mooa2023/demo-counter-app.git'
            }
        }

        stage('UNIT Testing'){
            
            steps{
                    sh 'mvn test'
            }
        }

        stage('Integration Testing'){
            
            steps{
                    sh 'mvn verify -DskipUnitTests'
            }
        }
    } 
}
