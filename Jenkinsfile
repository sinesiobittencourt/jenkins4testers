pipeline {
    agent any
        stages {
            stage("Build"){
                steps {
                sh 'git pull origin master'
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
            stage("Tests 2"){
                steps{
                sh "echo 'Simulando um teste'"
                }
            }
            
        }
}