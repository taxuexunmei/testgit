pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        unstable 'test hello world'
        sleep 10
        build(job: 'test', propagate: true, quietPeriod: 3)
      }
    }

    stage('second') {
      parallel {
        stage('second') {
          steps {
            sleep 4
          }
        }

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
  environment {
    name = 'smith'
  }
}