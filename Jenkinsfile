pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat label: 'Build artifact', script: 'echo "This is Jenkins build %BUILD_NUMBER% on branch %BRANCH_NAME%" > Build.txt'

		archiveArtifacts '*.txt'
            }
        }
    }
} 
