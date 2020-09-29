pipeline{
  agent any
  stage{
    stage ('Build'){
      steps{
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/train-schedule.zip'
      }
    }
  }
}
