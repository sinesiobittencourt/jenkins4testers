pipeline {
    agent any
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
        }                     
}