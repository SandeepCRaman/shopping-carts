pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
// this is a groovy script

    tools{
       maven 'maven' 
    }
    

    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'mvn package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
