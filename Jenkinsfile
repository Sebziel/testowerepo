pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'this is $BUILD_NUMBER of $DEMO'
      }
    }

  }
  environment {
    DEMO = 'demovalue1'
  }
}