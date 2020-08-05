pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout master
                git pull
                git checkout -b release-branch4
                git branch -a
                git push origin release-branch4
                """
            }
        }
    }
}
