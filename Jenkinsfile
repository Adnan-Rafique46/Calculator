pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
            echo 'test'
          }
        }

        stage('test par') {
          steps {
            echo 'test'
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}