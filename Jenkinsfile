pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo "this is $BUILD_NUMBER of $DEMO"'
      }
    }

    stage('stage2') {
      steps {
        writeFile(file: 'test-result.txt', text: 'passed')
      }
    }

    stage('post') {
      steps {
        archiveArtifacts 'test-results.txt'
      }
    }

  }
  environment {
    DEMO = 'demovalue1'
  }
}