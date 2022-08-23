pipeline {
    agent { label 'test-linux' }
    stages {
        stage ('git pull') {
            steps {
                git 'https://github.com/sramm24/website.git'
            }
        stage ('testing') {
            steps {
                sh 'echo "testing; in develop branch"'
            }
        }
        }
    }
}
