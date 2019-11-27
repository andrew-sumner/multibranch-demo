pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat label: 'Build artifact', script: 'echo "This is Jenkins build %BUILD_NUMBER%" > Build.txt'

		archiveArtifacts '*.txt'
            }
        }
    }
} 
