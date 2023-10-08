pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'https://github.com/elestopadov/java-example-apps.git', branch: 'main')
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            sleep 10
            echo 'deploy success'
          }
        }

        stage('deploy2') {
          steps {
            sleep 30
            echo 'deploy 2 success'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'test success!!!'
      }
    }

  }
}