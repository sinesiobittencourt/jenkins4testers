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
}

pipeline{
    post {
    failure {
        mail to: 'contato@sinesio.com.br',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "Something is wrong with ${env.BUILD_URL}"
    }
    }
}