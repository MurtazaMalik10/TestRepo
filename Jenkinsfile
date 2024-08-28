pipeline {

    agent any

    stages {

        stage('Build') {

            steps {

                script {

                    sh 'docker build -t public-image .'

                }

            }

        }

        stage('Deploy') {

            steps {

                script {

                    sh 'docker run -d -p 8081:80 public-image'

                }

            }

        }

    }

}
