pipeline {
    agent any
        stages {
            stage('Build') {
                parallel {
                    stage('Build Image') {
                      steps {
                        sh 'echo aaaaa>>a.txt'
                      }
                    }
                    
                  }
                post {
                    failure {
                        echo 'This build has failed. See logs for details.'
                    }
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
