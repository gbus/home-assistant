pipeline {
  agent {
    docker {
      image 'python:3.7-stretch'
      args '-v ha/config:/config'
    }

  }
  stages {
    stage('CreateEnv') {
      steps {
        sh 'test -e /venv3/bin/python || python -m venv /venv3'
      }
    }
  }
}