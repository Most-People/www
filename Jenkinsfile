pipeline {
  agent {
    node {
      label 'agent01'
    }

  }
  stages {
    stage('Source') {
      steps {
        git(branch: 'master', url: 'https://github.com/Most-People/www')
      }
    }

    stage('Build') {
      steps {
        tool 'gradle5'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Deploy Success"'
      }
    }

  }
}