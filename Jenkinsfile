pipeline{
    agent any
    
    stages{
        stage('hello-welcome'){
            steps{
                echo 'welocme to the mark antony'
                sh 'whoami'
                sh 'date'
                sh 'hostname'
            }
        }
        stage('build'){
            steps{
                echo 'application builded'
                sh 'pwd'
                sh 'python3 --version'
                sh 'python3 app.py'
                echo 'test the webiste'
            }
        }
    }
    post{
        success{
            echo 'completed'
        }
        failure{
            echo 'failed'
        }
    }
}
