pipeline {
    agent any
    stages {
         stage('Build 1') {
            steps {
                bat "mvn compile"
            }
        }
    stage('Build API') {
           steps {
               sh "nohup mvn spring-boot:run &"
               sleep(20)
              
           }
        }
    }
}
