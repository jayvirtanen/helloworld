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
    post {
        always {
            script {
                if (getContext(hudson.FilePath)) {
                    deleteDir()
                }
            }
        }
    }
}

