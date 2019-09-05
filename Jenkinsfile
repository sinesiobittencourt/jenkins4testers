pipeline {
    agent any
        stages {
            stage("Build"){
                steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
            }
            stage("Tests"){
                steps{
                sh "echo 'Simulando um teste'"
                }
            }
            
        }
    agent {
        docker { image 'node:7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}