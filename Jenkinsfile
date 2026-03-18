pipeline{
    agent any
    stages{
        stage ("one"){
            steps {
                sh "aws s3 mb s3://pipeline-assignment-4"
                sh "aws s3 cp index.html s3://pipeline-assignment-4/"
                sh "aws s3 sync . s3://pipeline-assignment-4"
                sh "aws s3 website s3://pipeline-assignment-4 --index-document index.html"
            }
        }
    }
}
