pipeline {
    agent any
    stages {
    stage ('Checkout') {
        git 'https://github.com/takwa7050/ICExam.git'
        }
    
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'apache-maven-3.6.2') {
                    bat 'mvn clean compile'
                }
            }
        }
        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'apache-maven-3.6.2') {
                    bat 'mvn test'
                }
            }
        }
        stage ('Install Stage') {
            steps {
                withMaven(maven : 'apache-maven-3.6.2') {
                    bat 'mvn install'
                }
            }
        }
    }
}
