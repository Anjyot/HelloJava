pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
               git branch: 'main', credentialsId: 'd6f8e71d-180f-44d6-8047-d8566458473d', url: 'https://github.com/Anjyot/HelloJava.git'
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
