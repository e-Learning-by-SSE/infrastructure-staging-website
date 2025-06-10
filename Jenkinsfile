pipeline {
    agent any

    stages {
        stage("Master deploy") {
            when {
                branch 'master'
            }
            steps {
                staging01ssh 'git --git-dir=/var/www/html2/.git --work-tree=/var/www/html2/ pull'
            }
        }
    }
}
