pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'First stage'
      }
    }

    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            echo 'Stage2'
          }
        }

        stage('Stage2a') {
          steps {
            echo 'Stage2a'
          }
        }

      }
    }

  }
}