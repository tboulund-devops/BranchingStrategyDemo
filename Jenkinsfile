pipeline {
    agent any
    stages {
        stage("Git merge") {
            steps {
                sh "git fetch --all"
                sh "git checkout master"
                sh "git pull"
                sh "git merge origin/${GIT_BRANCH}"
            }
        }
    }
}