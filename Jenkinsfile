pipeline {
    agent any
    stages {
        stage('clean-workspace') {
          steps {
           sh "git clean -n"
           }
        }
        stage('create branch') {
            steps {
                git branch: "release-branch8", credentialsId: github_repo, url: "https://github.com/linuxacademy/cicd-pipeline-train-schedule-cd.git"
                }
            }     
        }
    }
}
