pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'bash build.sh'
        emailext(subject: 'Build Status', body: 'This is the build status of current project', attachLog: true, from: 'reganshakya@gmail.com', to: 'regan@moco.com.np')
      }
    }

  }
}