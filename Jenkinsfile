pipeline {
  agent any
  stages {
    stage('Git Repo Code') {
      steps {
        git(url: 'https://github.com/nateprice18f/TechTalkCIDemo.git', branch: 'main', changelog: true)
      }
    }

    stage('test') {
      steps {
        echo 'test'
      }
    }

    stage('Release') {
      steps {
        echo 'release'
      }
    }

    stage('Deploy') {
      steps {
        pushToCloudFoundry(target: 'https://api.fr.cloud.gov', organization: 'sandbox-gsa', cloudSpace: 'nate.price', credentialsId: 'nate.price@gsa.gov')
      }
    }

  }
}