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
                git push -u origin branch5
                """
            }
        }
    }
}
