pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'github_repo', usernameVariable: 'USERNAME', passwordVariable: 'USERPASS')]) {
                git config --global credential.username {USERNAME}
                git config --global credential.helper "!echo password={PASSWORD}; echo"
                sh """
                git branch -a
                git checkout -b branch6
                git push origin branch6
                """
                }
            }
        }
    }
}
