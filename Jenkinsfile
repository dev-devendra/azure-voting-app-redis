pipeline {
    agent {
        docker {image 'node:1616-alpine'}
    }

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Docker Build') {
            steps {
                sh(script:'docker version')
            }
        }
    }
}
