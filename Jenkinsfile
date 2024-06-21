pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
               git branch: 'main', credentialsId: '2019cdc4-340a-481c-866f-903de8214d01', url: 'https://github.com/murali2023c/maven.git' 
            }
        }
        stage("build"){
            steps{
               sh 'sudo mvn --version'
            }
        }
        
    }
}
