pipeline{
    agent any    
    stages{
        //This is the actual stage
        stage('checkout'){
            steps {
                //this will fetch the code from the github
                git 'https://github.com/Ketan6969/Jenkins-Prac/blob/main/HelloWorld.java'       
            }
        }
        stage('compile'){
            steps{
                script{
                //this will compile the java code 
                sh 'javac HelloWorld.java'
                }
            }
        }
        stage('run'){
            steps{
                script{
                //This will run the java file
                sh 'java HelloWorld'
                }
            }
        }
   }
}