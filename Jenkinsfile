pipeline {
    agent any

    stages {
        stage('Code') {
            steps {
                echo '📝 Writing or preparing code...'
                // Simulate code step (optional)
                sh 'mkdir -p src && echo "public class App { public static void main(String[] args) { System.out.println(\\"Hello World\\"); }}" > src/App.java'
            }
        }

        stage('Build') {
            steps {
                echo '🔨 Compiling the code...'
                // Simulate build (for Java, using javac)
                sh 'javac src/App.java'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the application...'
                // Simulate deployment
                sh 'echo "Running app..." && java -cp src App'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
