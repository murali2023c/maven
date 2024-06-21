pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage('checkout'){
            steps{
               git branch: 'main', credentialsId: '2019cdc4-340a-481c-866f-903de8214d01', url: 'https://github.com/murali2023c/maven.git' 
            }
        }
        stage("version-check"){
            steps{
               sh 'mvn --version'
            }
        }
        stage("build"){
            steps{
               sh 'mvn install'
            }
        }
        
    }
}
