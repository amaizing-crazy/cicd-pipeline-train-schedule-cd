pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                echo 'Lets see'
                sh 'git checkout master'
                sh 'git branch feature/new-branch'
                sh 'git checkout feature/new-branch'
                sh 'git status'
            }
        }
    }
}
