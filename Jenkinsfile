pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Flaecken/spring-petclinic-angular.git'
            }
        }
         stage('Build') {
            steps {
                bat "mvn compile"
            }
        }
        stage('Test') {
            steps {
                bat "mvn test"
            }
            post {
                always {
                    junit '*/TEST.xml'
                }
            }
        }
              stage('Checkout') {
                steps {
                  git 'https://github.com/Flaecken/spring-petclinic-rest.git'
                }
              }
            stage('Build') {
      steps {
        bat "mvn compile"
      }
    }
    stage('Test') {
      steps {
        bat "mvn test"
      }
     post {
      always {
        junit '*/TEST.xml'
      }
     }
        }
    }
}
