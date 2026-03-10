pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/shubham221716/devops.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
            }
        }
    }
}
