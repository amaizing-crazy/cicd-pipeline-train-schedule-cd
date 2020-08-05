pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                echo 'Lets see'
                sh 'git checkout master'
                sh 'git branch release-branch0'
                sh 'git checkout release-branch0'
                sh 'git push origin release-branch0'
            }
        }
    }
}
