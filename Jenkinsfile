pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('parallel steps') {
      parallel {
        stage('compilation') {
          steps {
            sh 'echo Hello this is the compilation step'
          }
        }

        stage('test') {
          steps {
            echo 'testing'
          }
        }

      }
    }

    stage('deployment') {
      steps {
        echo 'Deploy'
      }
    }

  }
}
