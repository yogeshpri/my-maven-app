@Library('my-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/yogeshpri/jenkins-shared-lib'
            }
        }

        stage('Build with Maven') {
            steps {
                mavenBuild('clean package')
            }
        }
    }
}
