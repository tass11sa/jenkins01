pipeline {
    agent any
    tools {
        maven 'M2_HOME'
        jdk 'JAVA_HOME'
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build Maven') {
            steps {
                dir('DevOps-AppGestionDesProjets-main/backend') {
                    sh 'mvn compile'
                }
            }
        }
    }
}
