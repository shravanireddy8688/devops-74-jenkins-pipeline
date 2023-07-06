pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is developement'
      }
    }

    stage('test') {
      steps {
        echo 'this is testing'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build stage'
          }
        }

        stage('fixes') {
          steps {
            echo 'this is fixes'
          }
        }

        stage('oparate') {
          steps {
            echo 'this is oparate'
          }
        }

        stage('prod') {
          steps {
            echo 'this is production'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deploy'
          }
        }

      }
    }

  }
}