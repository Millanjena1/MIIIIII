pipeline{
    agent any
    stages{
         stage("checkout"){
            steps{
               sh 'git clone https://github.com/Millanjena1/java-code1.git'
            }
        }
        stage("move"){
            steps{
               sh 'cd ${WORKSPACE}/rwgwg/java-code1'
            }
        }
        stage("compile"){
            steps{
               sh 'mvn compile'
            }
        }
        stage("test"){
            steps{
                sh 'mvn test'
            }
        }
        stage("package"){
            steps{
               sh 'mvn package'
            }
        }
    }

}