pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build step completed'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is test step'
          }
        }
        stage('Opencv') {
          steps {
            echo 'opencv completed successfully'
          }
        }
        stage('Hardware') {
          steps {
            echo 'This is hardware step'
          }
        }
        stage('Compiler') {
          steps {
            echo 'This is compiler stage'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'This is deploy step'
      }
    }
  }
}