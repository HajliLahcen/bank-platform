pipeline {

    agent any

    stages {

        stage('Checkout') {

            steps {
                checkout scm
            }

        }

        stage('Verify Python') {

            steps {

                dir('api') {

                    sh 'python3 -m py_compile app.py'

                }

            }

        }

    }

}
