node {
    stage ('Checkout') {
        git 'https://github.com/takwa7050/ICExam.git'
        }
    
    stage ('Compile Stage') {
        def mvnHome = tool name: 'maven-3' , type: 'maven'
        sh "${mvnHome}/bin/mvn package" 
        }
}
