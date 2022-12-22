pipeline {
  agent {
    node {
      label 'centos7'
    }
  triggers {
  pollSCM '* * * * *'
}
  }
  stages {
    stage('checkout code') {
      steps {
        git(url: 'git@github.com:Spiceapps/NodeJS-EmptySiteTemplate.git', branch: 'master', credentialsId: 'jenkins_spiceapps', poll: true)
      }
    }

    stage('build') {
      steps {
        echo 'hello from build'
      }
    }

    stage('test') {
      steps {
        echo 'hello from test'
      }
    }

    stage('package') {
      steps {
        echo 'hello from package'
      }
    }

  }
}
