pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build Automation'
        sh './gradlew build --no-daemon'
      }
    }
    stage ('Archive the Artifact') {
      steps {
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
