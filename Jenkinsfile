pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "running build now bitches"
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
