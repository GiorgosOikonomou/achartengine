pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "error": {
            sh 'echo "george"'
            
          },
          "parallel step 2": {
            echo 'george'
            
          },
          "parallel step 3": {
            echo 'george'
            
          }
        )
      }
    }
    stage('pipeline stage 3') {
      steps {
        writeFile(file: 'test_file.txt', text: 'glksdfghjsolgj', encoding: 'utf-8')
      }
    }
  }
}