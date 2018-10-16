pipeline {
    agent any
        stages {
            stage('Build') {
                parallel {
                    stage('Build Image') {
                      steps {
                        sh 'docker build -f deploy.Dockerfile \
                        -t cd78/escc:latest .'
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
