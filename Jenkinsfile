pipeline{

    agent any

    stages{
        stage("compile"){
            steps{

                sh 'javac Test.java'
            }
        }
        stage("run"){
            steps{

                sh 'java Test'
            }
        }
    }

    post{

        always{
            sh 'echo "Always"'
        }

        success{
            sh 'echo "Build Success"'
        }
        failure{
            sh 'echo "Failure"'
        }
    }
}