pipeline{
    agent any
    tools{
        gradle 'gradle'
    }
    stages{
        stage("Clone code"){
            steps{
                git branch:'master', url:'https://github.com/Mary-softeng/java-todo.git'
                
            }
            
        }
        stage("Build code"){
            steps{
            sh 'gradle build'
        }
            
        }
        stage("Test Code"){
            steps{
                sh 'gradle test'
            }
        }
   
        
    }
}