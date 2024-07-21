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
        input(message: 'Are you sure you want to deploy ?', ok: 'Yes, I am sure')
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