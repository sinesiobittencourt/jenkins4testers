pipeline {
    agent {
        docker{
            image "ruby"
        }
    }
        stages {
            stage("Build"){
                steps {
                sh ' echo "oi"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
            }
            stage("git pull"){
                steps{
                sh "git pull origin master"
                }
            }                     
        }
}