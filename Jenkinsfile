pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'Build Stage'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build Stage'
          }
        }

        stage('Build 2 ') {
          steps {
            echo 'Build 2 Stage'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Stage'
      }
    }

    stage('Deploy On Prod') {
      steps {
        echo 'Deploy On Prod'
      }
    }

  }
}