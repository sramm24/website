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
        stage ('Docker build in PROD') {
            steps {
                sh 'sudo docker build /home/ubuntu/workspace/capstone1_master -t sramm24/capsproj'
            }
        }        
    }
}
