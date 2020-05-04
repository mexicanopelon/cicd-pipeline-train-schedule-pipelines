pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "running build now bitches"
                sh './gradlew build --no-deamon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
