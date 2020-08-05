pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout master
                git pull
                git checkout -b branch5
                git branch -a
                git push origin branch5
                """
            }
        }
    }
}
