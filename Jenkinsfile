@Library('web-service-helper-lib') _
pipeline {
    agent any

    stages {
        stage("Main deploy") {
            steps {
                staging01ssh 'git --git-dir=/var/www/html2/.git --work-tree=/var/www/html2/ pull'
            }
        }
    }
}
