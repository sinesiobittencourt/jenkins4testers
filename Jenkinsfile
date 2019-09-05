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
            stage("email"){
                post {
    failure {
        mail to: 'team@example.com',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "Something is wrong with ${env.BUILD_URL}"
    }
}

            }
            
        }
}