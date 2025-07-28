// Jenkinsfile for Eureka Microservices
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/your-username/eureka-microservices.git',
                    credentialsId: 'github-pat' // Replace with your actual Jenkins credential ID
            }
        }

        stage('Build') {
            steps {
                echo '🔨 Building Eureka microservice...'
                sh './mvnw clean package -DskipTests'  // or use mvn if wrapper not present
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                sh './mvnw test'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying Eureka microservice...'
                // Add deployment commands or scripts here
            }
        }
    }
}
