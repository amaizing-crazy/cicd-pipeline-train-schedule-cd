pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git checkout master
                git branch release-branch0
                git checkout release-branch0
                git push origin release-branch0
                """
            }
        }
    }
}
