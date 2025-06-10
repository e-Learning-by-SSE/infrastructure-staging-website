@Library('web-service-helper-lib') _
pipeline {
    agent any

    stages {
        stage("Main deploy") {
            steps {
                staging01ssh 'git --git-dir=/var/www/infrastructure-staging-website/.git --work-tree=/var/www/infrastructure-staging-website/ pull'
            }
        }
    }
}
