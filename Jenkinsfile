pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }

    stage('Backend') {
      parallel {
        stage('UnitTest') {
          steps {
            sh 'echo Backend'
          }
        }

        stage('Performance') {
          steps {
            sh 'echo Performance'
          }
        }

      }
    }

    stage('FrontEnd') {
      steps {
        sh 'echo FrontEnd'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}