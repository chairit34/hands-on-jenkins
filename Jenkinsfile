pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrom\''
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}
