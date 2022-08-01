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
        input(message: 'are you sure to deploy', ok: 'yes,i am sure')
        echo 'deployement completed'
      }
    }

    stage('notify for new build') {
      steps {
        echo 'new build completed successffly'
      }
    }

  }
}