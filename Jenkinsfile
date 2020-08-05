pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git branch -a
                git checkout -b branch6
                git push origin branch6
                """
            }
        }
    }
}
