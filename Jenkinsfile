pipeline {
  agent any
  stages {
    stage('maven') {
      steps {
        sh 'mvn -B -ntp -Dmaven.test.failure.ignore verify'
        junit '**/target/surefire-reports/TEST-*.xml'
      }
    }
  }
}
