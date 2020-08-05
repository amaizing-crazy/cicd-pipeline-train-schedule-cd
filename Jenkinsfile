pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout master
                git pull
                git branch -a
                git checkout branch5
                git push
                """
            }
        }
    }
}
