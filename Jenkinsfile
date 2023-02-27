pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'I want to devops'
      }
    }

    stage('Bulid') {
      steps {
        echo 'I want Bulid'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want test'
          }
        }

        stage('deploy') {
          steps {
            echo 'I want deploy'
          }
        }

      }
    }

  }
}