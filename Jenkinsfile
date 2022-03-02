pipeline{

    agent{ node{label 'master' } }
    tools{
        maven 'maven3.6.3'
        jdk 'java8'
    }

  
    stages{
    stage('Code Validate'){
        steps{
             sh 'mvn validate'
        }
    }
    stage('Code Compile'){
        steps{
             sh 'mvn compile'
        }
    }
    stage('Code test'){
        steps{
             sh 'mvn test'
        }
    }
    stage('Packge'){
        steps{
             sh 'mvn package'
        }
    }
}
}
