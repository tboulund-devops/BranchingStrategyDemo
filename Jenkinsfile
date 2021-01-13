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
        stage("Build") {
            steps {
                echo "Build stage - just a placeholder"
            }
        }
        stage("Test") {
            steps {
                echo "Test stage - just a placeholder"
            }
        }
        stage("Deliver") {
            steps {
                echo "Deliver stage - just a placeholder"
            }
        }
    }
}