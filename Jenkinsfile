pipeline {
    agent any
    stages {
        stage ("one") {
            steps {
                sh "rm -rf *"
                sh "cp -r index.html /var/www/html"
            }
        }
    }
}
