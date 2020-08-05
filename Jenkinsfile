pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'github_repo', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                sh """
                git config --global credential.username ${USERNAME}
                git config --global credential.helper "!echo password=${PASSWORD}; echo"
                git pull
                git branch -a
                git status
                git remote show origin 
                git checkout example-solution 
                git pull
                git checkout -b release-branch8
                git push origin release-branch8
                """
                }
            }
        }
    }
}
