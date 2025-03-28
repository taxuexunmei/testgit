pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        echo 'first'
      }
    }

    stage('second') {
      parallel {
        stage('second-2') {
          steps {
            echo 'second-2'
          }
        }

        stage('three-3') {
          steps {
            echo 'three-3'
          }
        }

      }
    }

    stage('three') {
      parallel {
        stage('three') {
          steps {
            echo '2563'
          }
        }

        stage('three-2') {
          steps {
            echo 'fsdfsdf'
          }
        }

        stage('error') {
          steps {
            echo 'sdfsdwe2'
          }
        }

      }
    }

    stage('email') {
      steps {
        echo '85203'
      }
    }

    stage('end') {
      steps {
        echo 'end'
      }
    }

  }
}