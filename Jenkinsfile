pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:lts-stretch-slim'
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