pipeline {
  agent any
  stages {
    stage('s1') {
      steps {
        echo 'Hello world'
      }
    }

    stage('s2') {
      parallel {
        stage('s2') {
          steps {
            echo 'Step 2'
          }
        }

        stage('s21') {
          steps {
            echo '"hello"'
          }
        }

      }
    }

    stage('T3') {
      steps {
        echo '"heelo"'
      }
    }

  }
}