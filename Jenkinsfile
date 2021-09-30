pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'At this stage we "Build" a docker image'
        sh 'npm install'
      }
    }

  }
}