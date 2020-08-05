pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                sh """
                git checkout example-solution
                git branch release-branch0
                git checkout release-branch0
                git push origin release-branch0
                """
            }
        }
    }
}
