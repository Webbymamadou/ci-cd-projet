pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh '''
                    docker run --rm \
                    -v "$WORKSPACE:/app" \
                    -w /app \
                    python:3.14-slim \
                    sh -c "pip install -r requirements.txt && pytest"
                '''
            }
        }
    }
}