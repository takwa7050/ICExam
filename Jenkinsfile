pipeline {
    agent any
    stages {
        stage ('Compile Stage') {

                    sh 'mvn clean compile'
               
        }
        stage ('Testing Stage') {

     
                    sh 'mvn test'
                }
            }
        }
        stage ('Install Stage') {
       
                   sh 'mvn install'
         
        }
    }
}
