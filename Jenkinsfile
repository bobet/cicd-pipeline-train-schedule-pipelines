
pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Starting building process'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
