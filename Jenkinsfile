pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Start Building'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Starting Test1'
          }
        }

        stage('Test2') {
          steps {
            echo 'Starting Test2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

    stage('Acknowledge Deployment') {
      steps {
        echo 'Deployed Successfully !'
      }
    }

  }
}
