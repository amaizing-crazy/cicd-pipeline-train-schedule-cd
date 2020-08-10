pipeline {
    agent any
    stages {
        stage('clean-workspace') {
          steps {
           sh "git clean -fdx"
           }
        }
        stage('create branch') {
            steps {
                git branch: "release-branch8", url: "https://github.com/linuxacademy/cicd-pipeline-train-schedule-cd.git"
                }
            }     
        }
    }
