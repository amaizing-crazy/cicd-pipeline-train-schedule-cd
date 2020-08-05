pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                echo 'Lets see'
                sh 'git checkout master'
                sh 'git branch release-branch1'
                sh 'git checkout release-branch1'
                sh 'git status'
            }
        }
    }
}
