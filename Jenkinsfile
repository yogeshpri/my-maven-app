@Library('my-shared-lib') _

pipeline {
    agent any

    stage('Checkout') {
    steps {
        git branch: 'main', url: 'https://github.com/yogeshpri/my-maven-app.git'
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
