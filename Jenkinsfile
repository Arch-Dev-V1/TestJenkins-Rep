/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:20.16.0-alpine3.20' } }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
