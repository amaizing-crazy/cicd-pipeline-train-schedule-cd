pipeline {
    agent any
    stages {
        stage('create branch') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'github_repo', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                sh """
                git config --global credential.username ${USERNAME}
                git config --global credential.helper "!echo password=${PASSWORD}; echo"
                git branch -a
                git remote update
                git fetch
                git checkout --track example-solution
                git branch -d branch6
                git checkout -b branch6
                git push origin branch6
                """
                }
            }
        }
    }
}
