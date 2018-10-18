pipeline {
    agent any
        stages {
            stage('Build') {
                steps {
                        sh 'echo aaaaa>>a.txt'
                }
                
                
            }
            stage('Test') {
                steps {
                    echo 'This is the Testing Stage'
                }
            }
            stage('Deploy') {
                steps {
                    echo 'This is the Deploy Stage'
                }
            }
        }
    }
