pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'Running automtion via Jenkins'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }        
    }
}
