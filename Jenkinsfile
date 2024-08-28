pipeline {

    agent any

    stages {

        stage('Build') {

            steps {

                script {

                    sh 'docker build -t my-image-name .'

                }

            }

        }

        stage('Deploy') {

            steps {

                script {

                    sh 'docker run -d -p 8080:80 my-image-name'

                }

            }

        }

    }

}
