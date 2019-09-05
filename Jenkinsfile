pipeline {
    agent any
        stages {
            stage("Build"){
                steps {
                sh 'cd /opt/lampp/htdocs/Public/addGoogleCalendar/'
                sh '''
                    git pull origin master
                    ls -lah
                '''
            }
            }
            stage("git pull"){
                steps{
                sh "git pull origin master"
                }
            }
            stage("add"){
                steps{
                sh "git add *"
                }
            }
            stage("commit"){
                steps{
                sh "git commit -m 'Update'"
                }
            }
            stage("push"){
                steps{
                sh "git push origin master"
                }
            }
            
            
        }
}