@Library('my-shared-lib@main') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yogeshpri/my-maven-app.git'
            }
        }

        stage('Build with Maven') {
            steps {
                mavenBuild()
            }
        }
    }
}

