pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo "this is $BUILD_NUMBER of $DEMO"'
      }
    }

  }
  environment {
    DEMO = 'demovalue1'
  }
}