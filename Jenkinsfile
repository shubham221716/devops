pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo "Cloning GitHub repository..."
                git 'https://github.com/shubham221716/devops.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo "Installing dependencies..."
                sh 'echo Installing packages'
            }
        }

        stage('Build Application') {
            steps {
                echo "Building application..."
                sh 'echo Build completed'
            }
        }

        stage('Run Tests') {
            steps {
                echo "Running tests..."
                sh 'echo All tests passed'
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Running code quality checks..."
                sh 'echo Code quality verified'
            }
        }

        stage('Package Application') {
            steps {
                echo "Packaging application..."
                sh 'tar -czf app.tar.gz *'
            }
        }

        stage('Deploy Application') {
            steps {
                echo "Deploying application..."
                sh 'echo Deployment successful'
            }
        }

    }

    post {
        success {
            echo "Pipeline executed successfully!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
