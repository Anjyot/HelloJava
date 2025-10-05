pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
               git branch: 'main', credentialsId: 'e7d1e391-a0ea-44b9-989c-b1ff572c6c1c', url: 'https://github.com/Anjyot/HelloJava.git'
            }
        }
         stage('Compile') {
            steps {
                bat 'javac Main.java'
            }
        }
         stage('Run') {
            steps {
                bat 'java Main'
            }
        }
    }
}
