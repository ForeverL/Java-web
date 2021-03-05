pipeline {
  agent any
  stages {
    stage('clean') {
      parallel {
        stage('clean1') {
          steps {
            echo 'clean'
          }
        }

        stage('clean2') {
          steps {
            sh '''echo "start clean"
sleep 3
echo "end clean"'''
            sleep 5
          }
        }

        stage('clean3') {
          steps {
            echo 'clean3'
          }
        }

      }
    }

    stage('package') {
      steps {
        echo 'package'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}