pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('test stages') {
      parallel {
        stage('test2') {
          steps {
            echo 'running tes2'
          }
        }

        stage('test1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployement completed'
      }
    }

  }
}