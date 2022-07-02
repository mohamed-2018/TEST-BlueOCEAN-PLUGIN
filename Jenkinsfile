pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
        retry(count: 3) {
          sh 'wwwwwwwwww'
        }

      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test1 running'
          }
        }

        stage('Test2') {
          steps {
            echo 'test2 running'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you wann deploy?', ok: 'Yes,I\'m Sure')
        echo 'Deployment Completed'
      }
    }

    stage('Notify for new deploy') {
      steps {
        echo 'Build Completed successfully'
      }
    }

  }
}