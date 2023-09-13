pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                archiveArtifacts artifacts: '*.html'
            }
        }
    }
}

