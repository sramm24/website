pipeline {
    agent { label 'prod-linux' }
    stages {
        stage ('git pull') {
            steps {
                git 'https://github.com/sramm24/website.git'
            }
        }
        stage ('testing') {
            steps {
                sh 'echo "testing; in master branch"'
            }
        }
        stage ('push to PROD') {
            steps {
                sh 'echo "Production; in master branch"'
            }
        }        
    }
}
