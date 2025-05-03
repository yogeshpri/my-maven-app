@Library('my-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone your Maven app code
                git 'https://github.com/yogeshpri/my-maven-app.git'
            }
        }

        stage('Build with Maven') {
            steps {
                // Call the shared library function
                mavenBuild('clean package')
            }
        }
    }
}
