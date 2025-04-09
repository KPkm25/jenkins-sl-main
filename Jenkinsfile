@Library('jenkins-sl')
pipeline {
  agent any

  stages {
    stage('Clone Repository') {
      steps {
        git url: 'https://github.com/KPkm25/jenkins-sl-main.git', branch: 'main' 
      }
    }
    
    stage('Build') {
      steps {
        sh 'echo "Building the application"'
      }
    }

    stage('Running Share Libraries') {
      steps {
        sh 'commonBuild()'
      }
    }

  }
}
