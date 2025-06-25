pipeline {
  agent any
  stages {
    stage('cleanup') {
      steps {
        sh 'docker system prune -a --volumes --force'
      }
    }
    stage('build image') {
      steps {
        sh 'docker build -t NikhilArya2017/python_jenkinsfile_Docker:8.5-204 .'
      }
    }
  }
}
