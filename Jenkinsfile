pipeline {
    agent{
        docker{
            image "ruby"
        }
    }
        stages {
            stage("Build"){
                steps {
                    sh 'bundle install'
                     }
            }
        }                     
}