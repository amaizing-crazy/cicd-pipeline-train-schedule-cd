pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout master
                git pull
                git checkout -b release-branch3
                git branch -a
                git push remote-repo release-branch3
                """
            }
        }
    }
}
