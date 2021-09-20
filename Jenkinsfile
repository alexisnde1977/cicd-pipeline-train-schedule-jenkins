pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation by alexis'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
