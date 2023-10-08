pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'https://github.com/elestopadov/java-example-apps.git', branch: 'main')
      }
    }

    stage('deploy') {
      steps {
        sleep 10
        echo 'deploy success'
      }
    }

    stage('test') {
      steps {
        echo 'test success!!!'
      }
    }

  }
}