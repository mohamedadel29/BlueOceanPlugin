pipeline {
  agent any
  stages {
    stage('bulid') {
      steps {
        echo 'hello'
      }
    }

    stage('test stages') {
      parallel {
        stage('test2') {
          steps {
            echo 'running test2'
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
        echo 'deploy'
      }
    }

  }
}