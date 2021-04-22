pipeline {
    agent any
    stages {
         stage('Build 1') {
            steps {
                bat "mvn compile"
            }
        }
              stage('Second Checkout') {
                steps {
                  git 'https://github.com/Flaecken/spring-petclinic-angular.git'
                }
              }
            stage('Build 2') {
      steps {
        bat "mvn compile"
      }
    }
    }
}
