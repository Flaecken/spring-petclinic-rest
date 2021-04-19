pipeline {
    agent any
    stages {
        stage('First Checkout') {
            steps {
                git 'https://github.com/Flaecken/spring-petclinic-rest.git'
            }
        }
         stage('Build 1') {
            steps {
                bat "mvn compile"
            }
        }
        /*stage('Test 1') {
            steps {
               bat "mvn test"
            }
            post {
                always {
                    junit '*//*TEST.xml'
               }
            }
        }*/
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
   /* stage('Test 2') {
      steps {
        bat "mvn test"
      }
     post {
      always {
        junit '*//*TEST.xml'
      }
     }
        } */
    }
}
