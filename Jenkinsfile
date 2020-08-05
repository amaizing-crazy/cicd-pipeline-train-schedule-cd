pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout master
                git pull
                git checkout example-solution
                git branch -a
                """
            }
        }
    }
}
